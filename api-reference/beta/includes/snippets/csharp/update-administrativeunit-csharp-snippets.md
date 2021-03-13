---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b88366dee1fb9b08ffe87c531b5fe3e801ff27b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "displayName-value",
    Description = "description-value",
    Visibility = "visibility-value"
};

await graphClient.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .UpdateAsync(administrativeUnit);

```