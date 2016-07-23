# numd

  > Склонение слов после числительных, для русского языка.

  * 1 рубль
  * 2 рубля
  * 5 рублей

## Установка

```go
import "github.com/xboston/numd-go"
```

## API

```go
numd.Decline(num, nominative, genitiveSingular, genitivePlural)
numd.DeclineLabel(num, nominative, genitiveSingular, genitivePlural)
```

Получаем полную форму в нужном склонении:

```go
price := numd.Decline(24, "рубль", "рубля", "рублей") // 24 рубля
length := numd.Decline(51, "метр", "метра", "метров") // 51 метр
```

Получаем только слово в нужном склонении:

```go
price := numd.DeclineLabel(24, "рубль", "рубля", "рублей") // рубля
length := numd.DeclineLabel(51, "метр", "метра", "метров") // метр
```

## Ссылки

 - [Документация](https://godoc.org/github.com/xboston/numd-go)
 - [Оригинальный проект](https://github.com/andrepolischuk/numd-go)

## License

  MIT
