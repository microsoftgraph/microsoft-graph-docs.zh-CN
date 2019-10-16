---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f374197fd762ad05afa69ecb63dd99d69881de16
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535582"
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