---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cf0702b42e4988f7e3d5b7becdcc34414be17de5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Reviewers["006111db-0810-4494-a6df-904d368bd81b"]
    .Request()
    .DeleteAsync();

```