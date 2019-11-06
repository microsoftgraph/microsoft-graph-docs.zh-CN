---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e85935c8556e9ab053f2992b925e44db11b84db6
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994752"
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

await graphClient.Me.Profile.EducationalActivities["{id}"]
    .Request()
    .UpdateAsync(educationalActivity);

```