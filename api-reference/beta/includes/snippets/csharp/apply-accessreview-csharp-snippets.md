---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 126a446a855f2e0ba9796537d7dfbb4497611a06
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794083"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .ApplyDecisions()
    .Request()
    .PostAsync();

```