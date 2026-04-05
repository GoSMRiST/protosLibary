# 📦 ProtosLib

Библиотека protobuf-контрактов для взаимодействия между сервисами.

Содержит **gRPC `.proto` файлы** и сгенерированный код, используемый в микросервисной архитектуре для стандартизации API и обмена данными.

---

## 🚀 Возможности

* 📡 Общие gRPC контракты для сервисов
* 🔄 Генерация кода для Go
* 🧩 Единая точка правды для API
* 📦 Переиспользование в разных сервисах
* ⚡ Упрощение интеграции между микросервисами

---

## 🛠️ Технологии

* **Protocol Buffers (protobuf)**
* **gRPC**
* **Go (protoc-gen-go, protoc-gen-go-grpc)**

---

## 📂 Структура проекта

```bash
.
├── proto/                 # Основные .proto файлы
│   ├── auth/
│   ├── user/
│   └── ...
├── gen/                   # Сгенерированный Go код
├── go.mod
└── go.sum
```

---

## ⚙️ Генерация кода

Убедитесь, что установлены:

```bash
protoc
protoc-gen-go
protoc-gen-go-grpc
```

Пример генерации:

```bash
protoc --go_out=. --go-grpc_out=. proto/**/*.proto
```

---

## 📡 Использование

Подключите библиотеку в ваш сервис:

```bash
go get github.com/GoSMRiST/protoslib
```

Импорт в коде:

```go
import "github.com/GoSMRiST/protoslib/gen/..."
```

---

## 👤 Автор

* GitHub: https://github.com/GoSMRiST
