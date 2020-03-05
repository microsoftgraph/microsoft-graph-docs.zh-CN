---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a66182d4be0eee8cf091394ccb8e9f6d900ee5a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivity = new EducationalActivity
{
    CompletionMonthYear = new Date(1900,1,1),
    EndMonthYear = new Date(1900,1,1),
    Institution = new InstitutionData
    {
        Description = "description-value",
        DisplayName = "displayName-value",
        Location = new PhysicalAddress
        {
            Type = PhysicalAddressType.Unknown,
            PostOfficeBox = "postOfficeBox-value",
            Street = "street-value",
            City = "city-value",
            State = "state-value",
            CountryOrRegion = "countryOrRegion-value",
            PostalCode = "postalCode-value"
        },
        WebUrl = "webUrl-value"
    },
    Program = new EducationalActivityDetail
    {
        Abbreviation = "abbreviation-value",
        Activities = "activities-value",
        Awards = "awards-value",
        Description = "description-value",
        DisplayName = "displayName-value",
        FieldsOfStudy = "fieldsOfStudy-value",
        Grade = "grade-value",
        Notes = "notes-value",
        WebUrl = "webUrl-value"
    },
    StartMonthYear = new Date(1900,1,1)
};

await graphClient.Me.Profile.EducationalActivities
    .Request()
    .AddAsync(educationalActivity);

```