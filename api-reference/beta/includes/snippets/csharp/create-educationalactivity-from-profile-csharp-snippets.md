---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90bab6294d81e857f569b923ac1029db9ed2a46253dad46cb6190db0f742ee90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104756"
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