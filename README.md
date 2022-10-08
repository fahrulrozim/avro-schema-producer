# avro-schema-producer

This is a repository for Session 8 of Data Engineer Fellowship in IYKRA. In this session, I was tasked to make an avro producer and consumer using `bitcoin_price_Training` dataset. You can get the dataset from this [link](https://classroom.google.com/u/0/c/NDg5ODMxNjk2MjM0/a/NTUyMzkzNjgzODgz/details?pli=1).

Pre-requisite:
1. Python 3.7 or later. Please note that using `confluent kafka` in python 3.8.8 windows OS might resulting in error DLL Cimpl file based on this [thread](https://github.com/confluentinc/confluent-kafka-python/issues/1186).
2. confluent_kafka. You can get that by using command `pip install confluent_kafka`.
3. avro. You can get that by using command `pip install avro-python3`.
4. requests. You can get that by using command `pip install requests`.

How to run:
1. Open your working file directory and navigate it in your terminal to use command `docker-compose up` to run file `docker-compose.yml`.
2. You can edit your key and value schema based on your choice in file `bitcoin_price_key.avsc` and `bitcoin_price_value.avsc`.
3. Run python file `avro_producer.py` with command `python avro_producer.py`.
4. Run python file `avro_consumer.py` with command `python avro_consumer.py`.
5. Simply kill every terminal if you're done running and use `docker-compose down` to delete all container.
