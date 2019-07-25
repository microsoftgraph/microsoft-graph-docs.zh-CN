---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e8184fa035985989c491300ab71b52ef41406f96
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewers = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Reviewers
    .Request()
    .GetAsync();

```