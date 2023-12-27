rabbitmqctl add_user newadmin s0m3p4ssw0rd

rabbitmqctl set_user_tags newadmin administrator

# set_permissions [-p vhostpath] {user} {conf} {write} {read}

rabbitmqctl set_permissions -p / newadmin "._" "._" ".\*"
