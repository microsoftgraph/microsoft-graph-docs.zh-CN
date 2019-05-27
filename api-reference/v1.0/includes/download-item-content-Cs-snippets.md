---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 633928dc0357c5f3715993b373140ae2280d498d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var items = await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = items.Content;

```