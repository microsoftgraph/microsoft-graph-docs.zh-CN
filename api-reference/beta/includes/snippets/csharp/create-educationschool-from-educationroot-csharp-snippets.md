---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 357f47f549e96b0f7c7ce0ecec4b5c791b5d3897
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714564"
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
    Fax = "+1 (253) 555-0101",
    Phone = "+1 (253) 555-0102"
};

await graphClient.Education.Schools
    .Request()
    .AddAsync(educationSchool);

```