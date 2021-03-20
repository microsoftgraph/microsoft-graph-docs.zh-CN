---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdbfe3dd71e3ba840916c0a5aa1124ccd4779aef
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myDecisions = await graphClient.AccessReviews["{accessReview-id}"].MyDecisions
    .Request()
    .GetAsync();

```