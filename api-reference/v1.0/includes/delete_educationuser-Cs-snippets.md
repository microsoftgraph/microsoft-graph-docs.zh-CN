---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a0a350786874bb7faea8c5d040cdf7fd3e430541
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```