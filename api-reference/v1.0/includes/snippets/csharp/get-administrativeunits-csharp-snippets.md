---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e61cb946723461936b58a7f3ea27149306f48f06
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnits = await graphClient.Directory.AdministrativeUnits
    .Request()
    .GetAsync();

```