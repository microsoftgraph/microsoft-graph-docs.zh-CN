---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 641bbf734e579ab1f9ac710899f59bf536edd7b6
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49846019"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviews = await graphClient.AccessReviews
    .Request()
    .Filter("businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68',")
    .Skip(0)
    .Top(100)
    .GetAsync();

```