---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0e00e718b6941ee211bfacc6982609b457eb278
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .Stop()
    .Request()
    .PostAsync();

```