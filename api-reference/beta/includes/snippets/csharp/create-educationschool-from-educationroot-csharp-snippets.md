---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94c6c40a91ce09937778ab33bb2c5ed21e8aa3d1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37554895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam High School",
    Description = "Magnate school for the arts. Los Angeles School District",
    Status = "String",
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