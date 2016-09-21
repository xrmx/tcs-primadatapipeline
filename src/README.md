# La mia prima data pipeline

## setup api

```
cd api
go build
```

## setup pipeline

```
virtualenv venv
. ./venv/bin/activate 
pip install wheel
cd pipeline
python setup.py install
cd -
```

## setup caravel

https://github.com/airbnb/caravel/blob/master/docs/installation.rst#making-your-own-build

## quickstart

Da un terminale facciamo partire le api

```
./api/api
```

Dall'altro creiamo il db ed eseguiamo la pipeline per un giorno
```
. ./venv/bin/activate

python createdb.py

luigi.sh 2016-09-20
```
