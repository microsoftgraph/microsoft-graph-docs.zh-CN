---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a37bf299e71cc57642ccca9b4f11178a4e1f3042
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders.Delta()
    .Request()
    .GetAsync();

```