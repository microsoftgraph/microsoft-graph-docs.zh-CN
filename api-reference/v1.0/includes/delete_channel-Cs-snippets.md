---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 690db678ce07c8b29957bc91a2d1150dc8ceecf8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Channels["{id}"]
    .Request()
    .DeleteAsync();

```