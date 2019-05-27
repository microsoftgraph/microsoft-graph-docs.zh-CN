---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e429d8f324c334d5a7f5c2bd609ccae3f76b1a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{item-id}"]
    .Checkout()
    .Request()
    .PostAsync();

```