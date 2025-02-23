prepare_install &&

install -dvm 755 /usr/share/SecLists &&
cp -rv Discovery Fuzzing IOCs Miscellaneous Passwords /usr/share/SecLists/ &&
cp -rv Pattern-Matching Payloads Usernames Web-Shells /usr/share/SecLists/ &&

mkdir -p /usr/share/wordlists
ln -sfv ../SecLists /usr/share/wordlists/
