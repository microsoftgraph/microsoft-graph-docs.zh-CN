---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4f001e058a5f16930339cf7f48dd3bca4419aaa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"].Reviewers["{accessReviewReviewer-id}"]
    .Request()
    .DeleteAsync();

```