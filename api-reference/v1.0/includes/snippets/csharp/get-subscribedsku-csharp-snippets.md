---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27243f32ce1690c651ae094c08e99b2c75415507
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618799"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSku = await graphClient.SubscribedSkus["{id}"]
    .Request()
    .GetAsync();

```