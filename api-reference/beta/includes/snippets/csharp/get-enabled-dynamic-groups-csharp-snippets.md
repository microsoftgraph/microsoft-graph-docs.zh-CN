---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2a26682a4c7bf6fe21bbb050468a7ff407282ac
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59998189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'")
    .Select("id,membershipRule,membershipRuleProcessingState")
    .GetAsync();

```