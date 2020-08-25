---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d62230fa4ed48fb11d981f704cfa94e9f707a3c
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var aAMkADIyAAAAABrJAAA= = await graphClient.Me.Todo.Lists.AAMkADIyAAAAABrJAAA=
    .Request()
    .GetAsync();

```