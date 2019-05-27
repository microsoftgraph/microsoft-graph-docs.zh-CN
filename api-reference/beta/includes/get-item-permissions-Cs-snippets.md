---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 994ab8cf6d7762268d9714e72036817ccbae6ae3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Me.Drive.Items["{item-id}"].Permissions
    .Request()
    .GetAsync();

```