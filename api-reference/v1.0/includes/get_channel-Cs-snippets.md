---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c8962445fc41eb169eff91bd17c6c88e7e693682
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{id}"].Channels["{id}"]
    .Request()
    .GetAsync();

```