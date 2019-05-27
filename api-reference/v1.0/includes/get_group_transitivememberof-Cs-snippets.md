---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ec497cedfc8d21e493c1fe275f1a1d5ceaa9eaf4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Groups["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```