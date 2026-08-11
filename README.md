# Илья Сухов / Ilya Sukhov

**RU** *(ниже)* · [**EN**](#english)

---

<a id="russian"></a>

## 🇷🇺 Русский

> Мне нравится понимать, как всё устроено на самом деле — **под API, под абстракциями, в рантайме.** Сейчас это в основном Go.

Go — мой основной язык, и большую часть времени я копаюсь в том, что под капотом: как планировщик рулит горутинами, когда GC даёт о себе знать, что реально делает мьютекс, пока две горутины дерутся за лок.

### 🎤 Доклад

**Внутреннее устройство мьютексов в Go** · [GoFunc](https://www.youtube.com/@GoFuncConf) · 2024

[![Доклад: Внутреннее устройство мьютексов в Go](https://i.ytimg.com/vi/qlft05-_rrU/hqdefault.jpg)](https://www.youtube.com/watch?v=qlft05-_rrU)

> Разобрал, как устроены мьютексы в Go изнутри: состояния, блокировка через atomic CAS, очередь waiters — и при каких условиях включается starvation mode.

👉 [Смотреть доклад](https://www.youtube.com/watch?v=qlft05-_rrU) · [Слайды](ССЫЛКА_НА_СЛАЙДЫ)

### Над чем разбирался

**Геометрия под нагрузкой** · `geo / ГИС`
Работал над бэкендом геоинформационного редактора, который отдаёт пользовательские геообъекты (полигоны, polyline) внешним сервисам. Самое интересное тут — **валидация пересечения polyline ∩ polygon**: дорогая вычислительная геометрия в горячем пути. Чтобы понять, где реально тратится время, обернул проверку в кастомный пространственный кеш и убрал повторные пересчёты.
`Go` `computational geometry`

### Стек

![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) ![gRPC](https://img.shields.io/badge/gRPC-244c5a?logo=grpc) ![Kafka](https://img.shields.io/badge/Kafka-231F20?logo=apachekafka&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)

### На связи

- **Email:** [ilya+github@suhov.site](mailto:ilya+github@suhov.site)

Рад обсудить Go internals, геометрию под нагрузкой или просто технически поболтать.

---

<a id="english"></a>

## 🇬🇧 English

> I like understanding how things really work — **under the API, under the abstractions, in the runtime.** Lately that's mostly Go.

Go is my main language, and I spend most of my time digging into what's under the hood: how the scheduler manages goroutines, when the GC makes itself felt, what a mutex actually does while two goroutines fight over a lock.

### 🎤 Talk

**Internals of Mutexes in Go** · [GoFunc](https://www.youtube.com/@GoFuncConf) · 2024 · *(in Russian)*

[![Talk: Internals of Mutexes in Go](https://i.ytimg.com/vi/qlft05-_rrU/hqdefault.jpg)](https://www.youtube.com/watch?v=qlft05-_rrU)

> A walkthrough of how Go mutexes work inside: mutex states, atomic CAS locking, the waiters queue — and when starvation mode kicks in.

👉 [Watch the talk](https://www.youtube.com/watch?v=qlft05-_rrU) · [Slides](SLIDES_LINK)

### What I dug into

**Geometry under load** · `geo / GIS`
Worked on the backend of a geo-information editor that serves user-defined geo-objects (polygons, polylines) to external services. The most interesting part was **polyline ∩ polygon intersection validation**: expensive computational geometry sitting in the hot path. To understand where the time actually goes, I wrapped the check in a custom spatial cache and eliminated redundant recomputation.
`Go` `computational geometry`

### Tech stack

![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) ![gRPC](https://img.shields.io/badge/gRPC-244c5a?logo=grpc) ![Kafka](https://img.shields.io/badge/Kafka-231F20?logo=apachekafka&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)

### Get in touch

- **Email:** [ilya+github@suhov.site](mailto:ilya+github@suhov.site)

Happy to chat about Go internals, geometry under load, or just talk shop.
