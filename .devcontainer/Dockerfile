FROM rust:latest
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
    libudev-dev \
    gdb-multiarch \
    picocom \
    openocd \
    make \
    binutils-multiarch \
    binutils-arm-none-eabi \
    llvm

RUN cargo install probe-rs-tools
RUN rustup target add thumbv7em-none-eabihf