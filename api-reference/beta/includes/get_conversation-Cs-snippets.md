---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef6caa3f9a541be3e7e525818b5079343c77bf26
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = await graphClient.Groups["{id}"].Conversations["{id}"]
    .Request()
    .GetAsync();

```