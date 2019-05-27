---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 74feb3e07eefdfa63b14f7cd644863b352828ca3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Activities["{activity-id}"]
    .Request()
    .DeleteAsync();

```