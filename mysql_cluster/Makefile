REMOTE_HOST=192.168.31.241
all: rsync

rsync:
	rsync -rvl root@${REMOTE_HOST}:/opt/workspace/* ./

clean:
	docker-compose stop; docker-compose rm -f

run:
	docker-compose up -d

.PHONY: rsync all run clean


