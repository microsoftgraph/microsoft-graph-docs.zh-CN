---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c8178971e37b68db8a704e11cc3da1e4c9ce4518af0019009798935cad83692
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409602"
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