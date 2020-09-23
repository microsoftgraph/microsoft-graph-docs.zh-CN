---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba43221084f0a295fabe542177f5e10e92f31dd0
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223613"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "Seattle District Technical Schools",
    Description = "Seattle district technical schools administration",
    Visibility = "HiddenMembership"
};

await graphClient.Directory.AdministrativeUnits
    .Request()
    .AddAsync(administrativeUnit);

```