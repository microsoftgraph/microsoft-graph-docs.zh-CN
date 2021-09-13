---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e52a61d1a07627c1bc96003d4f14ac5aa250186364abd0f06ef4b7b71ef7445
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "String",
    Description = "String",
    ExternalSource = EducationExternalSource.Sis,
    ExternalSourceDetail = "String",
    PrincipalEmail = "String",
    PrincipalName = "String",
    ExternalPrincipalId = "String",
    LowestGrade = "String",
    HighestGrade = "String",
    SchoolNumber = "String",
    ExternalId = "String",
    Phone = "String",
    Fax = "String",
    CreatedBy = new IdentitySet
    {
    },
    Address = new PhysicalAddress
    {
    }
};

await graphClient.Education.Schools
    .Request()
    .AddAsync(educationSchool);

```