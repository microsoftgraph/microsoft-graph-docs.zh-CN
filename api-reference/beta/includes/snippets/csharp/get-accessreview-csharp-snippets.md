---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23db8bf9f3dbe6662f430e02d8106c5199bca6a3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"]
    .Request()
    .GetAsync();

```