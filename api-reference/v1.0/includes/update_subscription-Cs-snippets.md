---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07559c71a1afeee4818c5bc9cfe7dc47955d9d26
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ExpirationDateTime = "2016-11-22T18:23:45.9356913Z"
};

await graphClient.Subscriptions["{id}"]
    .Request()
    .UpdateAsync(subscription);

```