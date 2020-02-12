---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f374197fd762ad05afa69ecb63dd99d69881de16
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
};

var removeLicenses = new List<Guid>()
{
    Guid.Parse("skuId-value-1"),
    Guid.Parse("skuId-value-2")
};

await graphClient.Groups["1ad75eeb-7e5a-4367-a493-9214d90d54d0"]
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```