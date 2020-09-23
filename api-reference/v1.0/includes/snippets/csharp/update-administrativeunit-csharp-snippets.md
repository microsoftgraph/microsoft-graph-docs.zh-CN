---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a70b2390dcd80d2c01efea4f428e3f0caab306f4
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223683"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "displayName-value",
    Description = "description-value",
    Visibility = "visibility-value"
};

await graphClient.Directory.AdministrativeUnits["{id}"]
    .Request()
    .UpdateAsync(administrativeUnit);

```