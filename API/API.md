# API Reference

1. [Интерфейс скриптов 1.0 (на языке TypeScript)](scripts.om.d.ts)
1. [Интерфейс Common](common.md)
1. [Окружение](env.md)
1. [Представления](views.md)
	1. [Измерения](dimensions.md)
	1. [Манипуляция элементами](elementsManipulator.md)
	1. [Низкоуровневый доступ к клеткам и кубам](cubeCell.md)
	1. [Синхронизация мультикубов и справочников](sync.md)
1. [Экспорт и импорт](exportImport.md)
1. [Файловые системы](fs.md)
1. [Файлы CSV](csv.md)
1. [Оптимизационные запросы](optimization.md)
1. [Коннекторы](connectors.md)
	1. [Реляционные БД](relationalDB.md)
	1. [MongoDB](mongoDB.md)
	1. [HTTP](http.md)
	1. [WinAgent](winAgent.md)
1. [Уведомление пользователя](notifications.md)
1. [Цепочки скриптов](scriptChains.md)
1. [Web API сервисы](apiService.md)

### Интерфейс OM<a name="om"></a>
```ts
interface OM {
	readonly common: Common;
	readonly environment: Environment;
	readonly multicubes: Multicubes;
	readonly times: Times;
	readonly versions: Versions;
	readonly lists: Lists;
	readonly filesystems: Filesystems;
	readonly optimization: Optimization;
	readonly connectors: Connectors;
	readonly notifications: Notifications.Manager;
        readonly variables: Variables;
}

var om: OM;
```
Интерфейс `OM` являет собой набор интерфейсов, предоставляющих API cкриптов 1.0 через глобальную переменную `om`.

&nbsp;

```js
readonly common: Common
```
Ссылка на интерфейс [`Common`](./common.md#common).

&nbsp;

```js
readonly environment: Environment
```
Ссылка на интерфейс [`Environment`](./env.md#environment).

&nbsp;

```js
readonly multicubes: Multicubes
```
Ссылка на интерфейс [`Multicubes`](./views.md#multicubes).

&nbsp;

```js
readonly times: Times
```
Ссылка на интерфейс [`Times`](./dimensions.md#times).

&nbsp;

```js
readonly versions: Versions
```
Ссылка на интерфейс [`Versions`](./dimensions.md#versions).

&nbsp;

```js
readonly lists: Lists
```
Ссылка на интерфейс [`Lists`](./dimensions.md#lists).

&nbsp;

```js
readonly filesystems: Filesystems
```
Ссылка на интерфейс [`Filesystems`](./fs.md#filesystems).

&nbsp;

```js
readonly optimization: Optimization
```
Ссылка на интерфейс [`Optimization`](./optimization.md#optimization).

&nbsp;

```js
readonly connectors: Connectors
```
Ссылка на интерфейс [`Connectors`](./connectors.md#connectors).

&nbsp;

```js
readonly notifications: Notifications.Manager
```
Ссылка на интерфейс [`Notifications.Manager`](./notifications.md#manager).

&nbsp;

```js
readonly variables: Variables;
```
Ссылка на интерфейс [`Variables`](./variables.md#variables).

&nbsp;

[Оглавление](../README.md)
