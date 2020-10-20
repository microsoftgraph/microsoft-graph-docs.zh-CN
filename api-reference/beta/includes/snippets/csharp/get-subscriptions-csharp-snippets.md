---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 340db99262c2c9d3473c9c32f990888433be36ee
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscriptions = await graphClient.Subscriptions
    .Request()
    .GetAsync();

```