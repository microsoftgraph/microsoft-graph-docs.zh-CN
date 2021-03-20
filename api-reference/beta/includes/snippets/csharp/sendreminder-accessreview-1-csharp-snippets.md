---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0634052c1099e764b82ad428f4f57cfd18188b5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .SendReminder()
    .Request()
    .PostAsync();

```