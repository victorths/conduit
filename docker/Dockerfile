FROM dart:stable

COPY packages/ packages/
COPY melos.yaml melos.yaml
RUN dart pub global activate -spath packages/cli
RUN dart pub global activate melos
RUN dart pub global run melos:melos cache-source
