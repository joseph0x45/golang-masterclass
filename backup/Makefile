CONTAINER_NAME=postgres17

setup-db:
	docker run --name $(CONTAINER_NAME) -p 5432:5432 -e POSTGRES_USER=root -e POSTGRES_PASSWORD=secret -d postgres:17-alpine

into-db:
	docker exec -it $(CONTAINER_NAME) psql -U root
