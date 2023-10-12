FROM ubuntu:22.04

RUN mkdir -p /srv

RUN mkdir -p /srv/data

RUN mkdir -p /srv/modules

RUN mkdir -p /srv/modules/js-module

RUN apt-get update && apt-get install -y curl libatomic1

RUN curl -Lo /srv/altv-server https://cdn.alt-mp.com/server/release/x64_linux/altv-server

RUN curl -Lo /srv/data/clothes.bin https://cdn.alt-mp.com/data/release/data/clothes.bin

RUN curl -Lo /srv/data/vehmods.bin https://cdn.alt-mp.com/data/release/data/vehmods.bin

RUN curl -Lo /srv/data/vehmodels.bin https://cdn.alt-mp.com/data/release/data/vehmodels.bin

RUN curl -Lo /srv/data/pedmodels.bin https://cdn.alt-mp.com/data/release/data/pedmodels.bin

RUN curl -Lo /srv/modules/libjs-bytecode-module.so https://cdn.alt-mp.com/js-bytecode-module/release/x64_linux/modules/libjs-bytecode-module.so

RUN curl -Lo /srv/ AltV.Net.Host.dll https://cdn.alt-mp.com/coreclr-module/release/x64_linux/AltV.Net.Host.dll

RUN curl -Lo /srv/ AltV.Net.Host.runtimeconfig.json https://cdn.alt-mp.com/coreclr-module/release/x64_linux/AltV.Net.Host.runtimeconfig.json

RUN curl -Lo /srv/modules/libcsharp-module.so https://cdn.alt-mp.com/coreclr-module/release/x64_linux/modules/libcsharp-module.so

RUN curl -Lo /srv/modules/js-module/libjs-module.so https://cdn.alt-mp.com/js-module/release/x64_linux/modules/js-module/libjs-module.so

RUN curl -Lo /srv/modules/js-module/libnode.so.102 https://cdn.alt-mp.com/js-module/release/x64_linux/modules/js-module/libnode.so.102

RUN chmod +x /srv/altv-server

WORKDIR /srv

CMD ./altv-server

