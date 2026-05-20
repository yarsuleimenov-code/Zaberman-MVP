# Zaberman Operational Pricing Platform

## Описание проекта

Внутренняя платформа для расчёта стоимости перевозок, управления estimate/invoice, eBOL и операционной логистики компании Zaberman.

Система предназначена для автоматизации расчётов при interstate-перевозках крупногабаритных, тяжёлых и хрупких грузов.

Проект объединяет:

- pricing engine
- operational dashboard
- vehicle allocation
- packaging logic
- eBOL workflow
- estimate/invoice generation
- cost breakdown
- warehouse/storage logic

---

# Цели системы

## Бизнес-цели

- Уменьшение ручных расчётов
- Стандартизация pricing logic
- Снижение ошибок при estimate
- Повышение прозрачности расчётов
- Ускорение обработки заказов
- Формирование единой operational platform

---

# Основные функции

## Pricing Engine

- Автоматический расчёт стоимости перевозки
- Расчёт interstate / pickup / delivery stages
- Dynamic variables
- Margin calculation
- Fuel calculation
- Labor calculation
- Packaging calculation
- Storage calculation
- Insurance calculation

---

## Logistics Constraints

- Non-stackable items
- Fragile items
- Crating logic
- Effective volume calculation
- Vehicle recommendation
- Multi-order consolidation

---

## eBOL System

- Электронный BOL
- Список items
- Фото предметов
- Pickup / delivery checkboxes
- Damage notes
- Signatures
- Item comments

---

## Operational Features

- Автоматический подбор vehicle
- Расчёт distance/zones
- Toll calculation
- Parking/ticket fees
- Storage services
- Stair fees
- Exclusive delivery

---

# Архитектура MVP

## Frontend

- HTML
- Tailwind CSS
- Chart.js

---

## Backend (planned)

- Node.js / Python
- REST API
- PostgreSQL

---

## Integrations

- Kommo CRM
- Stripe / Square
- Google Maps API
- Email/SMS services

---

# Структура MVP

## Основные экраны

### Dashboard
Operational overview и KPI.

---

### New Calculation
Создание estimate и расчёт стоимости.

---

### Items Management
Управление item list, packaging, photos, constraints.

---

### Cost Breakdown
Детализация расчёта стоимости.

---

### eBOL
Pickup / delivery execution workflow.

---

### Variables
Управление pricing variables и formula settings.

---

# Основные сущности системы

- Lead
- Customer
- Estimate
- Order
- Shipment
- Item
- Vehicle
- Route
- Invoice
- Payment
- eBOL

---

# Текущий статус

Проект находится на стадии:

## MVP / Wireframe / Business Architecture

---

# Roadmap

## Phase 1

- Pricing engine
- Estimate generation
- Vehicle allocation
- Packaging logic
- eBOL lite
- Variables system

---

## Phase 2

- Scheduling
- Dispatch workflows
- Warehouse operations
- Route planning

---

## Phase 3

- Driver mobile app
- AI recommendations
- Route optimization
- Real-time tracking

---

# Основные ограничения MVP

На текущем этапе:

- отсутствует backend
- отсутствует authentication
- отсутствует live integration
- отсутствует real-time dispatching
- отсутствует route optimization

---

# Ценность проекта

Система проектируется как единая operational platform для логистических перевозок с высокой вариативностью грузов и сложной pricing logic.

Основной акцент:
- гибкость pricing engine
- прозрачность cost calculation
- operational scalability
- минимизация ручной работы

---

# Repository Structure

```plaintext
/docs
/screenshots
/assets
/index.html
/items.html
/breakdown.html
/ebol.html
/variables.html
README.md
