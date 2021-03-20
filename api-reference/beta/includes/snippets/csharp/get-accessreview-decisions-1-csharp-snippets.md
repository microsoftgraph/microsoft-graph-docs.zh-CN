---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ea98f2b29da47a5d7b034ef14861daa37a6f397
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943165"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.AccessReviews["{accessReview-id}"].Decisions
    .Request()
    .GetAsync();

```