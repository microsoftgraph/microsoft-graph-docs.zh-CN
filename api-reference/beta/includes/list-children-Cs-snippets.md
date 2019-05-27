---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 01d6c26977f056a8c8d6cff431ff39463a67eb77
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Drives["{drive-id}"].Items["{item-id}"].Children
    .Request()
    .GetAsync();

```