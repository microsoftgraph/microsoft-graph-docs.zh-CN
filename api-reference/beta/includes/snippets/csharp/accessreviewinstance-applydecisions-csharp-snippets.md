---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 417258f70f7c730cc7179b412eda40dc0130c89f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["04e5c3b2-9db2-40d3-a204-128f4956ae8e"].Instances["70463350-742e-4909-bfa5-bc23447bd002"]
    .ApplyDecisions()
    .Request()
    .PostAsync();

```