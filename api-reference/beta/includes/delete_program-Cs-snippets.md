---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ed3748eb165161e9fedfc705f1889631879b4283
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437606"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Programs["7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"]
    .Request()
    .DeleteAsync();

```