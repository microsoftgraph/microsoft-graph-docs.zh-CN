---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b8fde04c45a421639c98901ffcf7b742d9fe393
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479500"
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