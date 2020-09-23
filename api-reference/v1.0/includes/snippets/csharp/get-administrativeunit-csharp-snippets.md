---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c16dce93d5645f81598abf4b90440950f455043f
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Directory.AdministrativeUnits["{id}"]
    .Request()
    .GetAsync();

```