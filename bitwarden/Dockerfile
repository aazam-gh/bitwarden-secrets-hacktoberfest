FROM ubuntu:18.04

RUN apt-get update && apt-get install -y \
    curl \
    unzip

RUN curl -O https://github.com/bitwarden/sdk/releases/download/bws-v0.3.1/bws-x86_64-unknown-linux-gnu-0.3.1.zip && unzip bws-x86_64-unknown-linux-gnu-0.3.1.zip && export PATH=/this/directory:$PATH
RUN SECRET_1=$(bws secret get 8d020a96-a7c5-4808-9cc4-b0ac00eb2ad9 --access-token $ACCESS_TOKEN | jq '.value')
RUN SECRET_2=$(bws secret get b93ad2a1-9298-4de0-9bfc-b0ac00eb403c --access-token $ACCESS_TOKEN | jq '.value')
RUN SECRET_3=$(bws secret get 814c8119-4188-4b28-9dfa-b0ac00eb5533 --access-token $ACCESS_TOKEN | jq '.value')