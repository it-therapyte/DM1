
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Содержание

- [Спецификация форматов данных](#%D1%81%D0%BF%D0%B5%D1%86%D0%B8%D1%84%D0%B8%D0%BA%D0%B0%D1%86%D0%B8%D1%8F-%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%82%D0%BE%D0%B2-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)
  - [О документе](#%D0%BE-%D0%B4%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B5)
  - [Формат файлов](#%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%82-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2)
  - [Структуры данных, принимаемых программой Feasibility](#%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D1%8B-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85-%D0%BF%D1%80%D0%B8%D0%BD%D0%B8%D0%BC%D0%B0%D0%B5%D0%BC%D1%8B%D1%85-%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BE%D0%B9-feasibility)
- [diagnosis.csv](#diagnosiscsv)
  - [<a name="patientId"></a>* Property `patientId`](#a-namepatientida-property-patientid)
  - [<a name="visitId"></a>* Property `visitId`](#a-namevisitida-property-visitid)
  - [<a name="code"></a>* Property `code`](#a-namecodea-property-code)
  - [<a name="type"></a>* Property `type`](#a-nametypea-property-type)
  - [<a name="name"></a>* Property `name`](#a-namenamea-property-name)
  - [<a name="charactersitic"></a>* Property `charactersitic`](#a-namecharactersitica-property-charactersitic)
  - [<a name="date"></a>* Property `date`](#a-namedatea-property-date)
- [examinations.csv](#examinationscsv)
  - [<a name="patientId"></a>* Property `patientId`](#a-namepatientida-property-patientid-1)
  - [<a name="visitId"></a>* Property `visitId`](#a-namevisitida-property-visitid-1)
  - [<a name="name"></a>* Property `name`](#a-namenamea-property-name-1)
  - [<a name="medRefCode"></a>* Property `medRefCode`](#a-namemedrefcodea-property-medrefcode)
  - [<a name="result"></a>* Property `result`](#a-nameresulta-property-result)
  - [<a name="resultNumerical"></a>* Property `resultNumerical`](#a-nameresultnumericala-property-resultnumerical)
  - [<a name="date"></a>* Property `date`](#a-namedatea-property-date-1)
- [medical-tests.csv](#medical-testscsv)
  - [<a name="patientId"></a>* Property `patientId`](#a-namepatientida-property-patientid-2)
  - [<a name="visitId"></a>* Property `visitId`](#a-namevisitida-property-visitid-2)
  - [<a name="testName"></a>* Property `testName`](#a-nametestnamea-property-testname)
  - [<a name="testParameter"></a>* Property `testParameter`](#a-nametestparametera-property-testparameter)
  - [<a name="testCode"></a>* Property `testCode`](#a-nametestcodea-property-testcode)
  - [<a name="textResult"></a>* Property `textResult`](#a-nametextresulta-property-textresult)
  - [<a name="value"></a>* Property `value`](#a-namevaluea-property-value)
  - [<a name="units"></a>* Property `units`](#a-nameunitsa-property-units)
  - [<a name="lowerLimit"></a>* Property `lowerLimit`](#a-namelowerlimita-property-lowerlimit)
  - [<a name="upperLimit"></a>* Property `upperLimit`](#a-nameupperlimita-property-upperlimit)
  - [<a name="date"></a>* Property `date`](#a-namedatea-property-date-2)
- [patients.csv](#patientscsv)
  - [<a name="patientId"></a>* Property `patientId`](#a-namepatientida-property-patientid-3)
  - [<a name="gender"></a>* Property `gender`](#a-namegendera-property-gender)
  - [<a name="yearOfBirth"></a>* Property `yearOfBirth`](#a-nameyearofbirtha-property-yearofbirth)
  - [<a name="menopause"></a>* Property `menopause`](#a-namemenopausea-property-menopause)
  - [<a name="menopauseAge"></a>* Property `menopauseAge`](#a-namemenopauseagea-property-menopauseage)
  - [<a name="deathDate"></a>* Property `deathDate`](#a-namedeathdatea-property-deathdate)
  - [<a name="healthCareOrgId"></a>* Property `healthCareOrgId`](#a-namehealthcareorgida-property-healthcareorgid)
- [procedures.csv (opt)](#procedurescsv-opt)
  - [<a name="patientId"></a>* Property `patientId`](#a-namepatientida-property-patientid-4)
  - [<a name="visitId"></a>* Property `visitId`](#a-namevisitida-property-visitid-3)
  - [<a name="name"></a>* Property `name`](#a-namenamea-property-name-2)
  - [<a name="date"></a>* Property `date`](#a-namedatea-property-date-3)
- [therapy.csv](#therapycsv)
  - [<a name="patientId"></a>* Property `patientId`](#a-namepatientida-property-patientid-5)
  - [<a name="visitId"></a>* Property `visitId`](#a-namevisitida-property-visitid-4)
  - [<a name="prescriptions"></a>* Property `prescriptions`](#a-nameprescriptionsa-property-prescriptions)
  - [<a name="medRefCode"></a>* Property `medRefCode`](#a-namemedrefcodea-property-medrefcode-1)
  - [<a name="startDate"></a>* Property `startDate`](#a-namestartdatea-property-startdate)
  - [<a name="endDate"></a>* Property `endDate`](#a-nameenddatea-property-enddate)
  - [<a name="amount"></a>* Property `amount`](#a-nameamounta-property-amount)
  - [<a name="drugForm"></a>* Property `drugForm`](#a-namedrugforma-property-drugform)
  - [<a name="singleDose"></a>* Property `singleDose`](#a-namesingledosea-property-singledose)
  - [<a name="frequency"></a>* Property `frequency`](#a-namefrequencya-property-frequency)
  - [<a name="routeOfAdm"></a>* Property `routeOfAdm`](#a-namerouteofadma-property-routeofadm)
  - [<a name="durationDays"></a>* Property `durationDays`](#a-namedurationdaysa-property-durationdays)
- [visits.csv](#visitscsv)
  - [<a name="patientId"></a>* Property `patientId`](#a-namepatientida-property-patientid-6)
  - [<a name="visitId"></a>* Property `visitId`](#a-namevisitida-property-visitid-5)
  - [<a name="date"></a>* Property `date`](#a-namedatea-property-date-4)
  - [<a name="type"></a>* Property `type`](#a-nametypea-property-type-1)
  - [<a name="region"></a>* Property `region`](#a-nameregiona-property-region)
  - [<a name="department"></a>* Property `department`](#a-namedepartmenta-property-department)
  - [<a name="spec"></a>* Property `spec`](#a-namespeca-property-spec)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Спецификация форматов данных  

*(autogenerated - do not edit)*

## О документе

Документ для разработчиков и интеграторов продуктов, связанных с ПО DataMatrix.

## Формат файлов

На вход принимаются табличные данные в формате .csv.  
Обязательные требования к файлам:

  1. Названия файлов должны соответствовать названию схемы.  
  2. Названия колонок в файле должны совпадать с названиями полей из описания структуры.  
  3. Значения полей в каждой колонке должны быть в формате соответсвующего поля схемы.
Каждая строка будет валидироваться в соответствии с описанием формата.
  4. В качестве разделителя использются `;`

## Структуры данных, принимаемых программой Feasibility

# diagnosis.csv

**Title:** diagnosis.csv

| Type                      | `object`                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Additional properties** | [![badge](https://img.shields.io/badge/Any+type-allowed-green)](# "Additional Properties of any type are allowed.") |
|                           |                                                                                                                     |

**Description:** Диагнозы

| Property                             | Pattern | Type             | Deprecated | Definition                                | Title/Description        |
| ------------------------------------ | ------- | ---------------- | ---------- | ----------------------------------------- | ------------------------ |
| + [patientId](#patientId )           | No      | string           | No         | In ../_common-types.json#/$defs/patientId | ID пациента              |
| + [visitId](#visitId )               | No      | string           | No         | In ../_common-types.json#/$defs/visitId   | ID визита                |
| + [code](#code )                     | No      | string           | No         | -                                         | Код по МКБ-10            |
| - [type](#type )                     | No      | enum (of string) | No         | -                                         | Тип диагноза             |
| - [name](#name )                     | No      | string           | No         | -                                         | Название диагноза        |
| - [charactersitic](#charactersitic ) | No      | enum (of string) | No         | -                                         | Характер заболевания     |
| + [date](#date )                     | No      | string           | No         | -                                         | Дата постановки диагноза |
|                                      |         |                  |            |                                           |                          |

## <a name="patientId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `patientId`

**Title:** ID пациента

| Type           | `string`                               |
| -------------- | -------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/patientId |
|                |                                        |

## <a name="visitId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `visitId`

**Title:** ID визита

| Type           | `string`                             |
| -------------- | ------------------------------------ |
| **Defined in** | ../_common-types.json#/$defs/visitId |
|                |                                      |

## <a name="code"></a>![badge](https://img.shields.io/badge/Required-blue) Property `code`

**Title:** Код по МКБ-10

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="type"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `type`

**Title:** Тип диагноза

| Type | `enum (of string)` |
| ---- | ------------------ |
|      |                    |

Must be one of:
* "основной"
* "сопутствующий"
* "осложнение основного"

## <a name="name"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `name`

**Title:** Название диагноза

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="charactersitic"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `charactersitic`

**Title:** Характер заболевания

| Type | `enum (of string)` |
| ---- | ------------------ |
|      |                    |

**Description:** Только для полной выгрузки

Must be one of:
* "ранее установленное"
* "первичность не подтверждена"
* "впервые в жизни установленное хроническое"

## <a name="date"></a>![badge](https://img.shields.io/badge/Required-blue) Property `date`

**Title:** Дата постановки диагноза

| Type | `string` |
| ---- | -------- |
|      |          |

----------------------------------------------------------------------------------------------------------------------------

# examinations.csv

**Title:** examinations.csv

| Type                      | `object`                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Additional properties** | [![badge](https://img.shields.io/badge/Any+type-allowed-green)](# "Additional Properties of any type are allowed.") |
|                           |                                                                                                                     |

**Description:** Обследования

| Property                               | Pattern | Type   | Deprecated | Definition                                | Title/Description         |
| -------------------------------------- | ------- | ------ | ---------- | ----------------------------------------- | ------------------------- |
| + [patientId](#patientId )             | No      | string | No         | In ../_common-types.json#/$defs/patientId | ID пациента               |
| + [visitId](#visitId )                 | No      | string | No         | In ../_common-types.json#/$defs/visitId   | ID визита                 |
| + [name](#name )                       | No      | string | No         | -                                         | Наименование обследования |
| - [medRefCode](#medRefCode )           | No      | string | No         | -                                         | Код по справочнику        |
| - [result](#result )                   | No      | string | No         | -                                         | Результат текстовый       |
| - [resultNumerical](#resultNumerical ) | No      | string | No         | -                                         | Результат числовой        |
| + [date](#date )                       | No      | string | No         | -                                         | Дата обследования         |
|                                        |         |        |            |                                           |                           |

## <a name="patientId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `patientId`

**Title:** ID пациента

| Type           | `string`                               |
| -------------- | -------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/patientId |
|                |                                        |

## <a name="visitId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `visitId`

**Title:** ID визита

| Type           | `string`                             |
| -------------- | ------------------------------------ |
| **Defined in** | ../_common-types.json#/$defs/visitId |
|                |                                      |

## <a name="name"></a>![badge](https://img.shields.io/badge/Required-blue) Property `name`

**Title:** Наименование обследования

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="medRefCode"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `medRefCode`

**Title:** Код по справочнику

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="result"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `result`

**Title:** Результат текстовый

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="resultNumerical"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `resultNumerical`

**Title:** Результат числовой

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="date"></a>![badge](https://img.shields.io/badge/Required-blue) Property `date`

**Title:** Дата обследования

| Type | `string` |
| ---- | -------- |
|      |          |

----------------------------------------------------------------------------------------------------------------------------

# medical-tests.csv

**Title:** medical-tests.csv

| Type                      | `object`                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Additional properties** | [![badge](https://img.shields.io/badge/Any+type-allowed-green)](# "Additional Properties of any type are allowed.") |
|                           |                                                                                                                     |

**Description:** Лабораторные данные

| Property                           | Pattern | Type   | Deprecated | Definition                                | Title/Description          |
| ---------------------------------- | ------- | ------ | ---------- | ----------------------------------------- | -------------------------- |
| + [patientId](#patientId )         | No      | string | No         | In ../_common-types.json#/$defs/patientId | ID пациента                |
| + [visitId](#visitId )             | No      | string | No         | In ../_common-types.json#/$defs/visitId   | ID визита                  |
| + [testName](#testName )           | No      | string | No         | -                                         | Наименование анализа       |
| + [testParameter](#testParameter ) | No      | string | No         | -                                         | Параметр в анализе         |
| + [testCode](#testCode )           | No      | string | No         | -                                         | Код по справочнику         |
| - [textResult](#textResult )       | No      | string | No         | -                                         | Результат текстовый        |
| + [value](#value )                 | No      | number | No         | -                                         | Результат числовой         |
| - [units](#units )                 | No      | string | No         | -                                         | Только для полной выгрузки |
| - [lowerLimit](#lowerLimit )       | No      | number | No         | -                                         | Нижняя граница нормы       |
| - [upperLimit](#upperLimit )       | No      | number | No         | -                                         | Верхняя гарница нормы      |
| + [date](#date )                   | No      | string | No         | -                                         | Дата проведения анализа    |
|                                    |         |        |            |                                           |                            |

## <a name="patientId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `patientId`

**Title:** ID пациента

| Type           | `string`                               |
| -------------- | -------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/patientId |
|                |                                        |

## <a name="visitId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `visitId`

**Title:** ID визита

| Type           | `string`                             |
| -------------- | ------------------------------------ |
| **Defined in** | ../_common-types.json#/$defs/visitId |
|                |                                      |

## <a name="testName"></a>![badge](https://img.shields.io/badge/Required-blue) Property `testName`

**Title:** Наименование анализа

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="testParameter"></a>![badge](https://img.shields.io/badge/Required-blue) Property `testParameter`

**Title:** Параметр в анализе

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="testCode"></a>![badge](https://img.shields.io/badge/Required-blue) Property `testCode`

**Title:** Код по справочнику

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="textResult"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `textResult`

**Title:** Результат текстовый

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="value"></a>![badge](https://img.shields.io/badge/Required-blue) Property `value`

**Title:** Результат числовой

| Type | `number` |
| ---- | -------- |
|      |          |

## <a name="units"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `units`

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="lowerLimit"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `lowerLimit`

**Title:** Нижняя граница нормы

| Type | `number` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="upperLimit"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `upperLimit`

**Title:** Верхняя гарница нормы

| Type | `number` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="date"></a>![badge](https://img.shields.io/badge/Required-blue) Property `date`

**Title:** Дата проведения анализа

| Type | `string` |
| ---- | -------- |
|      |          |

----------------------------------------------------------------------------------------------------------------------------

# patients.csv

**Title:** patients.csv

| Type                      | `object`                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Additional properties** | [![badge](https://img.shields.io/badge/Any+type-allowed-green)](# "Additional Properties of any type are allowed.") |
|                           |                                                                                                                     |

**Description:** Демографические данные

| Property                               | Pattern | Type             | Deprecated | Definition                                  | Title/Description                             |
| -------------------------------------- | ------- | ---------------- | ---------- | ------------------------------------------- | --------------------------------------------- |
| + [patientId](#patientId )             | No      | string           | No         | In ../_common-types.json#/$defs/patientId   | ID пациента                                   |
| + [gender](#gender )                   | No      | enum (of string) | No         | -                                           | -                                             |
| + [yearOfBirth](#yearOfBirth )         | No      | number           | No         | In ../_common-types.json#/$defs/yearOfBirth | Год рождения                                  |
| - [menopause](#menopause )             | No      | enum (of string) | No         | -                                           | Только для полной выгрузки, только для женщин |
| - [menopauseAge](#menopauseAge )       | No      | string           | No         | -                                           | Только для полной выгрузки, только для женщин |
| - [deathDate](#deathDate )             | No      | string           | No         | -                                           | Только для полной выгрузки, Если известно     |
| - [healthCareOrgId](#healthCareOrgId ) | No      | string           | No         | -                                           | Только для полной выгрузки                    |
|                                        |         |                  |            |                                             |                                               |

## <a name="patientId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `patientId`

**Title:** ID пациента

| Type           | `string`                               |
| -------------- | -------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/patientId |
|                |                                        |

## <a name="gender"></a>![badge](https://img.shields.io/badge/Required-blue) Property `gender`

| Type | `enum (of string)` |
| ---- | ------------------ |
|      |                    |

Must be one of:
* "м"
* "ж"

## <a name="yearOfBirth"></a>![badge](https://img.shields.io/badge/Required-blue) Property `yearOfBirth`

**Title:** Год рождения

| Type           | `number`                                 |
| -------------- | ---------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/yearOfBirth |
|                |                                          |

| Restrictions |        |
| ------------ | ------ |
| **Minimum**  | &ge; 0 |
|              |        |

## <a name="menopause"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `menopause`

| Type | `enum (of string)` |
| ---- | ------------------ |
|      |                    |

**Description:** Только для полной выгрузки, только для женщин

Must be one of:
* "Да"
* "Нет"

## <a name="menopauseAge"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `menopauseAge`

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки, только для женщин

## <a name="deathDate"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `deathDate`

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки, Если известно

## <a name="healthCareOrgId"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `healthCareOrgId`

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

----------------------------------------------------------------------------------------------------------------------------

# procedures.csv (opt)

**Title:** procedures.csv (opt)

| Type                      | `object`                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Additional properties** | [![badge](https://img.shields.io/badge/Any+type-allowed-green)](# "Additional Properties of any type are allowed.") |
|                           |                                                                                                                     |

**Description:** Процедуры

| Property                   | Pattern | Type   | Deprecated | Definition                                | Title/Description      |
| -------------------------- | ------- | ------ | ---------- | ----------------------------------------- | ---------------------- |
| + [patientId](#patientId ) | No      | string | No         | In ../_common-types.json#/$defs/patientId | ID пациента            |
| + [visitId](#visitId )     | No      | string | No         | In ../_common-types.json#/$defs/visitId   | ID визита              |
| + [name](#name )           | No      | string | No         | -                                         | Наименование процедуры |
| + [date](#date )           | No      | string | No         | -                                         | Дата процедуры         |
|                            |         |        |            |                                           |                        |

## <a name="patientId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `patientId`

**Title:** ID пациента

| Type           | `string`                               |
| -------------- | -------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/patientId |
|                |                                        |

## <a name="visitId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `visitId`

**Title:** ID визита

| Type           | `string`                             |
| -------------- | ------------------------------------ |
| **Defined in** | ../_common-types.json#/$defs/visitId |
|                |                                      |

## <a name="name"></a>![badge](https://img.shields.io/badge/Required-blue) Property `name`

**Title:** Наименование процедуры

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="date"></a>![badge](https://img.shields.io/badge/Required-blue) Property `date`

**Title:** Дата процедуры

| Type | `string` |
| ---- | -------- |
|      |          |

----------------------------------------------------------------------------------------------------------------------------

# therapy.csv

**Title:** therapy.csv

| Type                      | `object`                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Additional properties** | [![badge](https://img.shields.io/badge/Any+type-allowed-green)](# "Additional Properties of any type are allowed.") |
|                           |                                                                                                                     |

**Description:** Лекарственная терапия

| Property                           | Pattern | Type   | Deprecated | Definition                                | Title/Description           |
| ---------------------------------- | ------- | ------ | ---------- | ----------------------------------------- | --------------------------- |
| + [patientId](#patientId )         | No      | string | No         | In ../_common-types.json#/$defs/patientId | ID пациента                 |
| + [visitId](#visitId )             | No      | string | No         | In ../_common-types.json#/$defs/visitId   | ID визита                   |
| + [prescriptions](#prescriptions ) | No      | string | No         | -                                         | Лекарственные назначения    |
| - [medRefCode](#medRefCode )       | No      | string | No         | -                                         | Код по справочнику          |
| - [startDate](#startDate )         | No      | string | No         | -                                         | Дата начала приёма          |
| - [endDate](#endDate )             | No      | string | No         | -                                         | Дата окончания приёма       |
| - [amount](#amount )               | No      | string | No         | -                                         | Количество                  |
| - [drugForm](#drugForm )           | No      | string | No         | -                                         | Форма                       |
| - [singleDose](#singleDose )       | No      | string | No         | -                                         | Доза на одни приём          |
| - [frequency](#frequency )         | No      | string | No         | -                                         | Частота приёма              |
| - [routeOfAdm](#routeOfAdm )       | No      | string | No         | -                                         | Путь введения               |
| - [durationDays](#durationDays )   | No      | string | No         | -                                         | Длительность приёмов в днях |
|                                    |         |        |            |                                           |                             |

## <a name="patientId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `patientId`

**Title:** ID пациента

| Type           | `string`                               |
| -------------- | -------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/patientId |
|                |                                        |

## <a name="visitId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `visitId`

**Title:** ID визита

| Type           | `string`                             |
| -------------- | ------------------------------------ |
| **Defined in** | ../_common-types.json#/$defs/visitId |
|                |                                      |

## <a name="prescriptions"></a>![badge](https://img.shields.io/badge/Required-blue) Property `prescriptions`

**Title:** Лекарственные назначения

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="medRefCode"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `medRefCode`

**Title:** Код по справочнику

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="startDate"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `startDate`

**Title:** Дата начала приёма

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="endDate"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `endDate`

**Title:** Дата окончания приёма

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="amount"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `amount`

**Title:** Количество

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="drugForm"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `drugForm`

**Title:** Форма

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="singleDose"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `singleDose`

**Title:** Доза на одни приём

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="frequency"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `frequency`

**Title:** Частота приёма

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="routeOfAdm"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `routeOfAdm`

**Title:** Путь введения

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="durationDays"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `durationDays`

**Title:** Длительность приёмов в днях

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

----------------------------------------------------------------------------------------------------------------------------

# visits.csv

**Title:** visits.csv

| Type                      | `object`                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Additional properties** | [![badge](https://img.shields.io/badge/Any+type-allowed-green)](# "Additional Properties of any type are allowed.") |
|                           |                                                                                                                     |

**Description:** Посещения

| Property                     | Pattern | Type             | Deprecated | Definition                                | Title/Description          |
| ---------------------------- | ------- | ---------------- | ---------- | ----------------------------------------- | -------------------------- |
| + [patientId](#patientId )   | No      | string           | No         | In ../_common-types.json#/$defs/patientId | ID пациента                |
| + [visitId](#visitId )       | No      | string           | No         | In ../_common-types.json#/$defs/visitId   | ID визита                  |
| + [date](#date )             | No      | string           | No         | -                                         | Дата визита                |
| - [type](#type )             | No      | enum (of string) | No         | -                                         | Только для полной выгрузки |
| - [region](#region )         | No      | string           | No         | -                                         | Регион                     |
| - [department](#department ) | No      | string           | No         | -                                         | Наименование отделения     |
| - [spec](#spec )             | No      | string           | No         | -                                         | Специализация врача        |
|                              |         |                  |            |                                           |                            |

## <a name="patientId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `patientId`

**Title:** ID пациента

| Type           | `string`                               |
| -------------- | -------------------------------------- |
| **Defined in** | ../_common-types.json#/$defs/patientId |
|                |                                        |

## <a name="visitId"></a>![badge](https://img.shields.io/badge/Required-blue) Property `visitId`

**Title:** ID визита

| Type           | `string`                             |
| -------------- | ------------------------------------ |
| **Defined in** | ../_common-types.json#/$defs/visitId |
|                |                                      |

## <a name="date"></a>![badge](https://img.shields.io/badge/Required-blue) Property `date`

**Title:** Дата визита

| Type | `string` |
| ---- | -------- |
|      |          |

## <a name="type"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `type`

| Type | `enum (of string)` |
| ---- | ------------------ |
|      |                    |

**Description:** Только для полной выгрузки

Must be one of:
* "амбулаторный"
* "госпитализация"

## <a name="region"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `region`

**Title:** Регион

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="department"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `department`

**Title:** Наименование отделения

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

## <a name="spec"></a>![badge](https://img.shields.io/badge/Optional-yellow) Property `spec`

**Title:** Специализация врача

| Type | `string` |
| ---- | -------- |
|      |          |

**Description:** Только для полной выгрузки

----------------------------------------------------------------------------------------------------------------------------
