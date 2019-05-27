---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3161612c828c3b53c0fdb590561fa8c2542d1ee0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .ApplyDecisions()
    .Request()
    .PostAsync();

```