---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fba0d2d7e99eee4a442cf1ae35fab172fe512b6
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513669"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
};

var removeLicenses = new List<Guid>()
{
    Guid.Parse("c7df2760-2c81-4ef7-b578-5b5392b571df"),
    Guid.Parse("b05e124f-c7cc-45a0-a6aa-8cf78c946968")
};

await graphClient.Groups["{group-id}"]
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```