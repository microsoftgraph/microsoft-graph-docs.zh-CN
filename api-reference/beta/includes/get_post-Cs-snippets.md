---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3d64ead973a051c5d3945e0ab5351a482b32642f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = await graphClient.Groups["0d75b8dc-c42d-44dd-890a-751a99c0589f"].Threads["AAQkAD8EJUmcWwTJi06Cew=="].Posts["AQMkADgAAAIJbQAAAA=="]
    .Request()
    .GetAsync();

```