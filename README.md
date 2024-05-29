 Огляд структури бази даних

1. **Студенти (Students)**
   - **StudentId** (integer)
   - **FirstName** (varchar)
   - **LastName** (varchar)
   - **PhoneNumber** (integer)
   - **StudentDormitoryID** (integer)
   - **RoomNumber** (integer)

2. **Платежі (Payments)**
   - **PaymentId** (integer)
   - **StudentId** (integer)
   - **DateOfPayment** (date)
   - **Sum** (integer)

3. **Кімнати (Rooms)**
   - **RoomId** (integer)
   - **NumberOfBeds** (integer)
   - **RoomStatus** (varchar)
   - **FloorNumber** (integer)
   - **StudentId** (integer)

4. **Розподіл Кімнат (RoomAllocations)**
   - **AllocationID** (integer)
   - **RoomNumber** (integer)
   - **FloorNumber** (integer)
   - **CheckInDate** (date)
   - **CheckOutDate** (date)

5. **Гуртожитки (Dormitories)**
   - **DormitoryID** (integer)
   - **Capacity** (integer)
   - **Address** (varchar)

 Вимоги для REST API

 Основні функціональні вимоги

1. **CRUD операції для студентів**
   - Створення нового студента
   - Отримання інформації про студента
   - Оновлення інформації про студента
   - Видалення студента

2. **CRUD операції для платежів**
   - Створення нового платежу
   - Отримання інформації про платіж
   - Оновлення інформації про платіж
   - Видалення платежу

3. **CRUD операції для кімнат**
   - Створення нової кімнати
   - Отримання інформації про кімнату
   - Оновлення інформації про кімнату
   - Видалення кімнати

4. **CRUD операції для розподілу кімнат**
   - Створення нового розподілу кімнати
   - Отримання інформації про розподіл кімнати
   - Оновлення інформації про розподіл кімнати
   - Видалення розподілу кімнати

5. **CRUD операції для гуртожитків**
   - Створення нового гуртожитку
   - Отримання інформації про гуртожиток
   - Оновлення інформації про гуртожиток
   - Видалення гуртожитку

 Ендпойнти для REST API

 Студенти (Students)

- **GET /students** - Отримати список всіх студентів
- **GET /students/{id}** - Отримати інформацію про конкретного студента
- **POST /students** - Створити нового студента
- **PUT /students/{id}** - Оновити інформацію про студента
- **DELETE /students/{id}** - Видалити студента

 Платежі (Payments)

- **GET /payments** - Отримати список всіх платежів
- **GET /payments/{id}** - Отримати інформацію про конкретний платіж
- **POST /payments** - Створити новий платіж
- **PUT /payments/{id}** - Оновити інформацію про платіж
- **DELETE /payments/{id}** - Видалити платіж

 Кімнати (Rooms)

- **GET /rooms** - Отримати список всіх кімнат
- **GET /rooms/{id}** - Отримати інформацію про конкретну кімнату
- **POST /rooms** - Створити нову кімнату
- **PUT /rooms/{id}** - Оновити інформацію про кімнату
- **DELETE /rooms/{id}** - Видалити кімнату

 Розподіл Кімнат (RoomAllocations)

- **GET /roomallocations** - Отримати список всіх розподілів кімнат
- **GET /roomallocations/{id}** - Отримати інформацію про конкретний розподіл кімнати
- **POST /roomallocations** - Створити новий розподіл кімнати
- **PUT /roomallocations/{id}** - Оновити інформацію про розподіл кімнати
- **DELETE /roomallocations/{id}** - Видалити розподіл кімнати

 Гуртожитки (Dormitories)

- **GET /dormitories** - Отримати список всіх гуртожитків
- **GET /dormitories/{id}** - Отримати інформацію про конкретний гуртожиток
- **POST /dormitories** - Створити новий гуртожиток
- **PUT /dormitories/{id}** - Оновити інформацію про гуртожиток
- **DELETE /dormitories/{id}** - Видалити гуртожиток
