cat rapido-trains.sql | docker exec -i rapido_train_mysql mysql -u rapidotrains --password=rapidotrains rapidotrains

UPDATE `core_config_data` SET `value` = replace(value, 'http://localhost/rapido-trains/', 'http://localhost:4000/')  