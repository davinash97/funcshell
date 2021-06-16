#!/bin/bash
# This file is a part of https://www.github.com/davinash97/funcshell
# Use it with Proper Credits, And Make sure to tag the repo.
print "\n\tShell Scripting made easy for you by DAvinash97@github\n" "invert"
# This file is a part of https://www.github.com/davinash97/funcshell

print() {
    if [[ ! ${1} ]]; then
        echo -e "\n\t\033[0;31mYou need to provide some argument\033[0m\n"
    else
        CLR="${2}"
        case $CLR in
        black)
            echo -e "\t\033[0;30m${1}\033[0m\n"
            ;;
        red)
            echo -e "\t\033[0;31m${1}\033[0m\n"
            ;;
        green)
            echo -e "\t\033[0;32m${1}\033[0m\n"
            ;;
        yellow)
            echo -e "\t\033[0;33m${1}\033[0m\n"
            ;;
        blue)
            echo -e "\t\033[0;34m${1}\033[0m\n"
            ;;
        magenta)
            echo -e "\t\033[0;35m${1}\033[0m\n"
            ;;
        cyan)
            echo -e "\t\033[0;36m${1}\033[0m\n"
            ;;
        grey)
            echo -e "\t\033[0;90m${1}\033[0m\n"
            ;;
        black_bg)
            echo -e "\t\033[0;40m${1}\033[0m\n"
            ;;
        red_bg)
            echo -e "\t\033[0;41m${1}\033[0m\n"
            ;;
        green_bg)
            echo -e "\t\033[0;42m${1}\033[0m\n"
            ;;
        yellow_bg)
            echo -e "\t\033[0;43m${1}\033[0m\n"
            ;;
        blue_bg)
            echo -e "\t\033[0;44m${1}\033[0m\n"
            ;;
        magenta_bg)
            echo -e "\t\033[0;45m${1}\033[0m\n"
            ;;
        cyan_bg)
            echo -e "\t\033[0;46m${1}\033[0m\n"
            ;;
        grey_bg)
            echo -e "\t\033[0;100m${1}\033[0m\n"
            ;;
        invert)
            echo -e "\t\e[7m${1}\e[27m\n"
            ;;
        *)
            echo -e "\t\033[0;39m${1}\033[0m\n"
            ;;
        esac
    fi
}

print_logo() {
    if [ ! ${1} ]; then
        print "You need to provide some argument..." "red"
    else
        if [ -f ${1} ]; then
            banner=$(cat ${1})
            print "${banner}" "${2}"
        else
            print "Oops! ${1} doesn't seem to be a file, Check again..." "red"
        fi
    fi
}

delete() {
    if [ ! ${1} ]; then
        print "Delete What?" "red"
    else
        if [ -d "${1}" ]; then
            print "Deleting dir ${1}"
            rm -rf "${1}"
            print "Successfully Deleted ${1}"
        elif [ -f "${1}" ]; then
            print "Deleting file ${1}"
            rm -f "${1}"
            print "Successfully Deleted ${1}"
        else
            print "${1} not found, so can't delete..." "red"
        fi
    fi
}

permission() {
    if [ ! ${1} ]; then
        print "Change Permission for?" "red"
    else
        if [ -f ${1} ] || [ -d ${1} ]; then
            print "Changing permissions for $2"
            sudo chmod -R $1 $2
        else
            print "Such thing doesn't Exist..." "red"
        fi
    fi
}

get_access() {
    if [ ! ${1} ]; then
        print "Get Access? Where?" "red"
    else
        if [ -f ${1} ] || [ -d ${1} ]; then
            sudo chown $USER:$USER $1
        else
            print "Such thing doesn't Exist..." "red"
        fi
    fi
}

create_dir() {
    if [ ! ${1} ]; then
        print "Can't Create Folder named Blank." "red"
    else
        if [ -d ${1} ]; then
            print "Folder ${1} already exist" "red"
        else
            print "Creating ${1} Folder"
            mkdir ${1}
        fi
    fi
}

create_file() {
    if [ ! ${1} ]; then
        print "Can't Create File named Blank" "red"
    else
        if [ ! ${2} ]; then
            if [ -f ${1} ]; then
                print "${1} already exist in the current directory" "red"
            else
                print "Creating File named ${1}"
                touch "${1}"
            fi
        else
            if [ -d ${2} ]; then
                cd ${2}
                if [ -f ${1} ]; then
                    print "${1} already exist inside ${2}" "red"
                else
                    touch ${1}
                fi
                cd ..
            else
                print "Folder doesn't exist, So"
                create_dir "${2}"
                cd ${2}
                print "Creating ${1} file"
                touch ${1}
                cd ..
            fi
        fi
    fi
}

write() {
    if [ ! ${1} ]; then
        print "Write what? Provide Something" "red"
    else
        if [ ! ${2} ]; then
            print "Write Where? Add Filename..." "red"
        elif [ ! -f ${2} ]; then
            print "${2} Doesn't Exist" "red"
            print "Creating..."
            create_file "${2}"
            print "Now Writing"
            print "${1}" >"${2}"
            print "Done..."
        else
            print "Writing"
            print "${1}" >"${2}"
            print "Done..."
        fi
    fi
}
