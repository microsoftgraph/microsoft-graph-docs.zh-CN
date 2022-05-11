---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1065d31cf0922868af6b2377a248b5084e27ba91
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327890"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationalActivity()
completionMonthYear := "Date"
requestBody.SetCompletionMonthYear(&completionMonthYear)
endMonthYear := "Date"
requestBody.SetEndMonthYear(&endMonthYear)
institution := msgraphsdk.NewInstitutionData()
requestBody.SetInstitution(institution)
institution.SetDescription(nil)
displayName := "Colorado State University"
institution.SetDisplayName(&displayName)
location := msgraphsdk.NewPhysicalAddress()
institution.SetLocation(location)
type := "business"
location.SetType(&type)
location.SetPostOfficeBox(nil)
street := "12000 E Prospect Rd"
location.SetStreet(&street)
city := "Fort Collins"
location.SetCity(&city)
state := "Colorado"
location.SetState(&state)
countryOrRegion := "USA"
location.SetCountryOrRegion(&countryOrRegion)
postalCode := "80525"
location.SetPostalCode(&postalCode)
webUrl := "https://www.colostate.edu"
institution.SetWebUrl(&webUrl)
program := msgraphsdk.NewEducationalActivityDetail()
requestBody.SetProgram(program)
abbreviation := "MBA"
program.SetAbbreviation(&abbreviation)
program.SetActivities(nil)
program.SetAwards(nil)
description := "Master of Business Administration with a major in Entreprenuership and Finance."
program.SetDescription(&description)
displayName := "Master of Business Administration"
program.SetDisplayName(&displayName)
program.SetFieldsOfStudy(nil)
grade := "3.9"
program.SetGrade(&grade)
program.SetNotes(nil)
webUrl := "https://biz.colostate.edu"
program.SetWebUrl(&webUrl)
startMonthYear := "Date"
requestBody.SetStartMonthYear(&startMonthYear)
result, err := graphClient.Me().Profile().EducationalActivities().Post(requestBody)


```