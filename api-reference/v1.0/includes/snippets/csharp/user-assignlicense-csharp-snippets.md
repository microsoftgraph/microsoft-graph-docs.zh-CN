---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 16f4d683ca6c48161b67d316543056824e5117a0
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
    new AssignedLicense
    {
        DisabledPlans = new List<Guid>()
        {
            Guid.Parse("11b0131d-43c8-4bbb-b2c8-e80f9a50834a")
        },
        SkuId = Guid.Parse("guid")
    }
};

var removeLicenses = new List<Guid>()
{
    Guid.Parse("bea13e0c-3828-4daa-a392-28af7ff61a0f")
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```