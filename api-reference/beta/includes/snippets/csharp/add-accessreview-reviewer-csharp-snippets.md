---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4cbe0d1663ecc301d7adb136b1a09f9eb9ba7b9a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711169"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewReviewer = new AccessReviewReviewer
{
    Id = "006111db-0810-4494-a6df-904d368bd81b"
};

await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Reviewers
    .Request()
    .AddAsync(accessReviewReviewer);

```