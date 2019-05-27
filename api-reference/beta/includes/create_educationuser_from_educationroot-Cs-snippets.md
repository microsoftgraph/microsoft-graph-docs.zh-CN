---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 38cf36e48906fa5d668d1d597321e0870aa897b0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    DisplayName = "Dion Matheson",
    GivenName = "Dion",
    MiddleName = null,
    Surname = "Matheson",
    Mail = "DionM@contoso.com",
    MobilePhone = "+1 (253) 555-0101",
    CreatedBy = new IdentitySet
    {
        User = new Identity
        {
            DisplayName = "Susana Rocha",
            Id = "14012"
        }
    },
    ExternalSource = EducationExternalSource.Sis,
    MailingAddress = new PhysicalAddress
    {
        City = "Los Angeles",
        CountryOrRegion = "United States",
        PostalCode = "98055",
        State = "CA",
        Street = "12345 Main St."
    },
    PrimaryRole = EducationUserRole.Student,
    ResidenceAddress = new PhysicalAddress
    {
        City = "Los Angeles",
        CountryOrRegion = "United States",
        PostalCode = "98055",
        State = "CA",
        Street = "12345 Main St."
    }
};

await graphClient.Education.Users
    .Request()
    .AddAsync(educationUser);

```