---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f23b55e6dc51bc1030cac9c547f3cc7d151dc566
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{id}"].Channels
    .Request()
    .GetAsync();

```