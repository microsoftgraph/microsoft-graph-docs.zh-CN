---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f1273b3af26aa182b90e7963bf8e5fea5d8d3b41
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
    new AssignedLicense
    {
        DisabledPlans = new List<String>()
        {
            "11b0131d-43c8-4bbb-b2c8-e80f9a50834a"
        },
        SkuId = "guid"
    }
};

var removeLicenses = new List<String>()
{
    "bea13e0c-3828-4daa-a392-28af7ff61a0f"
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```