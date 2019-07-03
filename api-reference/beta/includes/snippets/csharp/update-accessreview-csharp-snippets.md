---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4afd13dfcfc245a698e55c900308872b7aee1e45
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520899"
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