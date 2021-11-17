---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c4077be712552b17084912ae3a849c53b08e7bd1babd6b92e0cabedf9e0b330
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"].Reviewers["{accessReviewReviewer-id}"]
    .Request()
    .DeleteAsync();

```