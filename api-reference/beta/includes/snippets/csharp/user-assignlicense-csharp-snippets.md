---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00119ca29af1bd54a9d985c1abea4b22ce16d34db819cae57fedeaf3cec38e52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163766"
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
        SkuId = Guid.Parse("skuId-value-1")
    },
    new AssignedLicense
    {
        DisabledPlans = new List<Guid>()
        {
            Guid.Parse("a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235")
        },
        SkuId = Guid.Parse("skuId-value-2")
    }
};

var removeLicenses = new List<Guid>()
{
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```