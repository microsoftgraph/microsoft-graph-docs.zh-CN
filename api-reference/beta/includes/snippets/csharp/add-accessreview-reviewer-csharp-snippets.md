---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9908874166221aced38caeb4ee0f93f1df3f0509f2062f11eca9c6100c7c308
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewReviewer = new AccessReviewReviewer
{
    Id = "006111db-0810-4494-a6df-904d368bd81b"
};

await graphClient.AccessReviews["{accessReview-id}"].Reviewers
    .Request()
    .AddAsync(accessReviewReviewer);

```