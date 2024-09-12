export GOPROXY=https://proxy.golang.org
#export GOFLAGS="-buildmode=pie -trimpath"

go build -v -o gobuster . &&

prepare_install &&

install -Dvm0755 gobuster /usr/bin/gobuster
