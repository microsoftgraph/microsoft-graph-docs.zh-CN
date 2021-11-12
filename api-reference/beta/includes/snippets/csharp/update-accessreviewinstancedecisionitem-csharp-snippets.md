---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60517cf912758ff37c842fb2127e79511b55f78b6631b3ef1b46412119860a44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem
{
    Decision = "Approve",
    Justification = "This person is still on my team"
};

await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"].Decisions["{accessReviewInstanceDecisionItem-id}"]
    .Request()
    .UpdateAsync(accessReviewInstanceDecisionItem);

```