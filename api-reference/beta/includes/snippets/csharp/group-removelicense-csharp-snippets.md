---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4a18244d03c14795d4abd1e05331ea5e42444d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796346"
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

await graphClient.Groups["{group-id}"]
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```