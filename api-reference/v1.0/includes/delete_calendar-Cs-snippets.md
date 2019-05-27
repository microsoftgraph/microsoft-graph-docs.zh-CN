---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 168d963ab77e81f46725e5846653c8be2c6e8a12
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Calendar
    .Request()
    .DeleteAsync();

```