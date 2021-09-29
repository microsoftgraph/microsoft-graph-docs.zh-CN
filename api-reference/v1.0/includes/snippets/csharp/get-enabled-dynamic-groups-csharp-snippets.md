---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ba248da6cebdc0c87d7c273e13dc724ad24f15a
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996077"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'")
    .Select("id,membershipRule,membershipRuleProcessingState")
    .GetAsync();

```