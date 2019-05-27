---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d818ace631e591ea0ae53d75a939a1627dfc7394
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469510"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .SendReminder()
    .Request()
    .PostAsync();

```