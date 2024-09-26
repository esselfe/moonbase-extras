
if in_depends $MODULE go; then
    go build -v gochest.go
fi &&

if in_depends $MODULE rustc; then
    cargo build --release
fi &&

make &&

prepare_install &&

install -Dm755 chest /usr/bin/ &&

if in_depends $MODULE go; then
    install -m755 gochest /usr/bin/gochest
fi &&

if in_depends $MODULE python; then
    install -m755 chest.py /usr/bin/chest.py
fi &&

if in_depends $MODULE rustc; then
    install -m755 target/release/rschest /usr/bin/rschest
fi
