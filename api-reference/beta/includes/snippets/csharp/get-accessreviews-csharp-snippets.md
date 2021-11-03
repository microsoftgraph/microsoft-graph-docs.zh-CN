---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94caec3c4e3847bbead4b059fc26417c8deac8420341ff158709e274241ecde8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviews = await graphClient.AccessReviews
    .Request()
    .Filter("businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'")
    .Skip(0)
    .Top(100)
    .GetAsync();

```