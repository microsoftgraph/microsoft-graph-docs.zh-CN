---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7980c22e1ca4152e7ea3834909392864a0bf9331
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"]
    .Request()
    .GetAsync();

```