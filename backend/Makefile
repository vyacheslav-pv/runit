setup: prepare-env install db-migrate

install:
	npm install

db-migrate:
	npm run typeorm -- migration:run -d src/data-source.ts

db-generate:
	npm run typeorm -- migration:generate src/migrations -d src/data-source

db-revert:
	npm run typeorm -- migration:revert -d src/data-source.ts

db-refresh: db-revert db-migrate

db-create-migration:
	npm run typeorm migration:create src/migrations/$(NAME)

db-drop:
	npm run typeorm -- schema:drop -d src/data-source.ts

start:
	npm run start

start-prod:
	npm run start:prod

build:
	npm run build

lint:
	npm run lint

lint-fix:
	npm run lint-fix

test:
	npm test

test-e2e:
	npm run test:e2e

data-drop:
	npm run typeorm -- migration:revert -d src/data-source.ts

prepare-env:
	cp -n .env.example .env
