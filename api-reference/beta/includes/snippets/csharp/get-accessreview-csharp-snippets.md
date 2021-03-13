---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f674b72647280e5bafb04c23e23123e66f29bc4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796318"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = await graphClient.AccessReviews["{accessReview-id}"]
    .Request()
    .GetAsync();

```