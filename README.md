# MetronMataElang

## Build Metron

1. Pastikan sudah terinstall git dan juga maven versi 3.3.9

2. Download Project Git dari Metron
   > clone https://github.com/fadli7/incubator-metron

3. Build metron dengan menggunakan maven
   > cd incubator-metron

   > mvn -q -T 2C -DskipTests -PHDP-2.5.0.0 install

4. Buat Direktori Home Metron
   > sudo mkdir -p /usr/metron/0.3.1

   > export METRON_HOME=/usr/metron/0.3.1

5. Ekstrak package yang sudah di build ke dalam direktori $METRON_HOME
   > tar xf ./metron-analytics/metron-profiler-client/target/metron-profiler-client-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-analytics/metron-profiler/target/metron-profiler-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-analytics/metron-maas-service/target/metron-maas-service-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-management/target/metron-management-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-common/target/metron-common-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-indexing/target/metron-indexing-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-elasticsearch/target/metron-elasticsearch-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-pcap-backend/target/metron-pcap-backend-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-data-management/target/metron-data-management-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-enrichment/target/metron-enrichment-0.3.1-archive.tar.gz -C $METRON_HOME

   > tar xf ./metron-platform/metron-parsers/target/metron-parsers-0.3.1-archive.tar.gz -C $METRON_HOME

