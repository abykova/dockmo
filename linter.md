https://golangci-lint.run/usage/install/

# macOS

`brew install golangci-lint`

`brew upgrade golangci-lint`

# Go 1.16+
`go install github.com/golangci/golangci-lint/cmd/golangci-lint@v1.43.0`

# Go version < 1.16
`go get -u github.com/golangci/golangci-lint/cmd/golangci-lint@v1.43.0`

`golangci-lint --version`

`golangci-lint run`

------

Инструменты оптимизации структур в дополнение к линтеру: 

> aligncheck;
> 
> maligned.  

Для этого нужно просто подключить `maligned` в настройках `golangci-lint`, например из конфигурационного файла `. golangci.example.yml`:

```
linters-settings:
  maligned:
      # выводит структуру с более эффективной схемой распределения памяти или нет, false по умолчанию
      suggest-new: true
      
```

Подробнее здесь: https://golangci-lint.run/usage/configuration/.

Это средство контроля качества кода позволяет запускать проверку на наличие возможности для оптимизации не только в ручном режиме локально на компьютере разработчика, но и как встроенный инструмент в CI/CD.



