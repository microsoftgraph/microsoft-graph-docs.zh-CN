---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b8fde04c45a421639c98901ffcf7b742d9fe393
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537446"
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
        SkuId = "skuId-value-1"
    },
    new AssignedLicense
    {
        DisabledPlans = new List<String>()
        {
            "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235"
        },
        SkuId = "skuId-value-2"
    }
};

var removeLicenses = new List<String>()
{
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```