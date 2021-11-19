---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3d68c081066805b248cb699ee5482dc8be9539b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082327"
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
options := &msgraphsdk.EducationalActivitiesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().EducationalActivities().Post(options)


```