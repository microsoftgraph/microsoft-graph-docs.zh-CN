---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c78dd739c35654a38e27aff8a42ef96568eff3d0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226874"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam High School",
    Description = "Magnate school for the arts. Los Angeles School District",
    ExternalSource = EducationExternalSource.Sis,
    PrincipalEmail = "AmyR@fabrikam.com",
    PrincipalName = "Amy Roebuck",
    ExternalPrincipalId = "14007",
    HighestGrade = "12",
    LowestGrade = "9",
    SchoolNumber = "10002",
    Address = new PhysicalAddress
    {
        City = "Los Angeles",
        CountryOrRegion = "United States",
        PostalCode = "98055",
        State = "CA",
        Street = "12345 Main St."
    },
    ExternalId = "10002",
    Phone = "+1 (253) 555-0102"
};

await graphClient.Education.Schools
    .Request()
    .AddAsync(educationSchool);

```