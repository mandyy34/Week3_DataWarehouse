SELECT count(*) FROM precise-rite-412708.nytaxi.greentaxi_2022 -- 840402

select count(distinct(PULocationID)) FROM precise-rite-412708.nytaxi.greentaxi_2022 -- 6.41MB

select count(distinct(PULocationID)) FROM precise-rite-412708.nytaxi.greentaxi_2022 -- 6.41MB

select count(distinct(PULocationID)) FROM precise-rite-412708.nytaxi.external_greentaxi_2022

select count(*) FROM precise-rite-412708.nytaxi.greentaxi_2022 -- 1622

CREATE OR REPLACE TABLE precise-rite-412708.nytaxi.partitioned_greentaxi_2022 PARTITION BY (lpep_pickup_date) CLUSTER BY PUlocationID AS ( SELECT * FROM precise-rite-412708.nytaxi.greentaxi_2022 );

SELECT distinct(PULocationID) FROM precise-rite-412708.nytaxi.greentaxi_2022 where lpep_pickup_date between '2022-06-01' and '2022-06-30' -- 12.82mb

SELECT distinct(PULocationID) FROM precise-rite-412708.nytaxi.partitioned_greentaxi_2022 where lpep_pickup_date between '2022-06-01' and '2022-06-30' -- 1.12mb
