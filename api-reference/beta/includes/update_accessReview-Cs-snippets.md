---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4afd13dfcfc245a698e55c900308872b7aee1e45
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461981"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = new AccessReview
{
    DisplayName = "TestReview new name"
};

await graphClient.AccessReviews["006111db-0810-4494-a6df-904d368bd81b"]
    .Request()
    .UpdateAsync(accessReview);

```