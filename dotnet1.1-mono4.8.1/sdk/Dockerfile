FROM microsoft/dotnet:1.1-sdk

LABEL maintainer "Johnny Santos <johnnyadsantos@gmail.com>"

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF \
    && echo "deb http://download.mono-project.com/repo/debian wheezy-libjpeg62-compat main" | tee -a /etc/apt/sources.list.d/mono-xamarin.list \
    && echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/4.8.1 main" | tee -a /etc/apt/sources.list.d/mono-xamarin.list \
    && apt-get update -qq \
    && apt-get install \
        -y \
        --no-install-recommends \
        --no-install-suggests \
        mono-complete \
        msbuild \
        ca-certificates-mono \
        referenceassemblies-pcl \
        nuget \
    && nuget update -Self \
    && rm -rf /var/lib/apt/lists/* \
    && apt-get autoremove \
    && apt-get autoclean \
    && mkdir /app

WORKDIR /app

VOLUME /app
