---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd1ab578bfc13a586c713a8dd06b890e89dda3a5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("membershipRuleProcessingState eq 'On'")
    .Select("id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus")
    .GetAsync();

```