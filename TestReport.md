# Отчет о тестировании Credit Card Number Validator
## Краткое описание
15.09.2020 было проведено Функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:

  https://github.com/NataliaOleinik/CreditCardValidatorTest/issues/1

## Описание процесса тестирования
В процессе тестирования использовались следующие артефакты:

 1. Руководство по установке IntelliJ IDEA
 2. IntelliJ IDEA с кодом для тестирования валидации номеров банковских карт

В качестве тестовых данных использовались:
 
 1. Данные из Руководства по установке IntelliJ IDEA(https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md):

    Руководство по установке IntelliJ IDEA работает под систему Windows 10 Версия 1909(Сборка ОС 18363.1016) 64-разрядная ОС
    Приложение успешно запускается


 2. Данные с https://www.freeformatter.com/credit-card-number-generator-validator.html#fakeNumbers:

     Валидные номера:

         * 4485723667346848
         * 4485228158228414
         * 4532623143620506553
         * 36869721745699

     Невалидные номера:

         * 47765037632251925479
         * 2221007963346
         * 2720990215J48278
         * 5018673664-59176

     Тестовые данные подставлялись в код, взятый с лекции https://github.com/netology-code/javaqa-homeworks/tree/master/intro,
     вставленный IntelliJ IDEA

 ## Ожидаемый результат:

   * 4485723667346848  Result is OK
   * 4485228158228414  Result is OK
   * 4532623143620506553 Result is OK
   * 36869721745699  Result is OK

   * 47765037632251925479 Result is FAIL
   * 2221007963346  Result is FAIL
   * 2720990215J48278  Result is FAIL
   * 5018673664-59176  Result is FAIL


 ## Фактический Результат:

  * 4485723667346848  Result is OK
  * 4485228158228414  Result is OK
  * 4532623143620506553 Result is FAIL
  * 36869721745699  Result is FAIL


  * 47765037632251925479  Result is FAIL
  * 2221007963346  Result is FAIL
  * 2720990215J48278  Result is FAIL
  * 5018673664-59176  Result is FAIL

 ## Тестирование производилось в следующем окружении:
   Windows 10 Версия 1909(Сборка ОС 18363.1016) 64-разрядная ОС
   Java openjdk version "11.0.8" 2020-07-14