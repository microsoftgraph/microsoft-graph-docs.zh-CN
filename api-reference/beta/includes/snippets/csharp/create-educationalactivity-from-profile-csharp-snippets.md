---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f17b276399e8350f8fc842cd381c28b8948ad5ac
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821263"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivity = new EducationalActivity
{
    CompletionMonthYear = new Date(1900,1,1),
    EndMonthYear = new Date(1900,1,1),
    Institution = new InstitutionData
    {
        Description = null,
        DisplayName = "Colorado State University",
        Location = new PhysicalAddress
        {
            Type = PhysicalAddressType.Business,
            PostOfficeBox = null,
            Street = "12000 E Prospect Rd",
            City = "Fort Collins",
            State = "Colorado",
            CountryOrRegion = "USA",
            PostalCode = "80525"
        },
        WebUrl = "https://www.colostate.edu"
    },
    Program = new EducationalActivityDetail
    {
        Abbreviation = "MBA",
        Activities = null,
        Awards = null,
        Description = "Master of Business Administration with a major in Entreprenuership and Finance.",
        DisplayName = "Master of Business Administration",
        FieldsOfStudy = null,
        Grade = "3.9",
        Notes = null,
        WebUrl = "https://biz.colostate.edu"
    },
    StartMonthYear = new Date(1900,1,1)
};

await graphClient.Me.Profile.EducationalActivities
    .Request()
    .AddAsync(educationalActivity);

```