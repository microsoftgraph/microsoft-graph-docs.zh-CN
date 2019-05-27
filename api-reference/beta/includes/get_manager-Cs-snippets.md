---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 35d0af3bfa42f85c0b5ab350895a99f7b49d6ab9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Contacts["{id}"].Manager
    .Request()
    .GetAsync();

```