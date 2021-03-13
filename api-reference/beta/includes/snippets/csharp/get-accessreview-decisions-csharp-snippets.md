---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdbfe3dd71e3ba840916c0a5aa1124ccd4779aef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myDecisions = await graphClient.AccessReviews["{accessReview-id}"].MyDecisions
    .Request()
    .GetAsync();

```