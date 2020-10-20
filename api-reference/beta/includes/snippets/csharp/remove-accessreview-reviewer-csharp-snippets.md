---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf0702b42e4988f7e3d5b7becdcc34414be17de5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608597"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Reviewers["006111db-0810-4494-a6df-904d368bd81b"]
    .Request()
    .DeleteAsync();

```