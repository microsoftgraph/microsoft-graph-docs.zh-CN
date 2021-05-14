---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cea74b13953c3c3a1a6694c7d03366202e4f39b1
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474816"
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