---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: e971b8049e780f4609fdba8ddaa6811fdef610fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstance = await graphClient.IdentityGovernance.AccessReviews.Definitions["60860cdd-fb4d-4054-91ba-444404f3baa6"].Instances["12490cdb-6a18-4c08-ba2c-44442f0a0138"]
    .Request()
    .GetAsync();

```