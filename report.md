**Отчёт о тестировании Key Validator**

**Краткое описание**
08.03.2021 было проведено тестирование документации, тестирование установки и функциональное тестирование приложения Key Validator.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:

[Вывод результата работы приложения KeyValidator не соответствует описанию в руководстве использования](https://github.com/Keirahn/KeyValidatorCase1/issues/1)

[Ключи, указанные в руководстве использования KeyValidator как валидные, не проходят валидацию](https://github.com/Keirahn/KeyValidatorCase1/issues/2)

[Ключ, указанный в руководстве использования KeyValidator как невалидный, проходит валидацию](https://github.com/Keirahn/KeyValidatorCase1/issues/3)

**Описание процесса тестирования**

В качестве тестовых данных использовались [Инструкция по установке OpenJDK 11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md), [руководство использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)

В качестве демонстрации работы приложения KeyValidator руководство использования содержит два типа значений - валидные ключи и невалидные ключи.

_Валидные ключи:_

```
8f05e6a7-70e9-33d7-bfe7-b19eae0d8998  - ожидаемый результат "ОК"
80b427f8-92cd-3aae-ba04-3927fbe17c6  - ожидаемый результат "ОК"
b295bc63-9f03-3b4b-af80-969b39f8c262  - ожидаемый результат "ОК"
387eedc6-12e9-3b32-9881-63b6b5e85317  - ожидаемый результат "ОК"
c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180. - ожидаемый результат "ОК"
```

_Невалидные ключи:_

```
18252235-78e0-44a5-8720-556f0c7da17a - ожидаемый результат "FAIL" 
e66075b6-ddad-445e-baf6-161b3289522b - ожидаемый результат "FAIL" 
b6d53250-f07e-4352-a293-6102ddf7f1ca - ожидаемый результат "FAIL" 
c2bc778a-1cb9-46c6-b435-0489649d2a42 - ожидаемый результат "FAIL" 
2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1 - ожидаемый результат "FAIL" 
```

**Тестирование производилось в следующем окружении:**

- macOS 11.1 (20C69)
- openjdk version "11.0.10" 2021-01-19
- OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.10+9)
- OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.10+9, mixed mode)
