---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f30d9c0a60f2681f70f4c6456228b736c980dfc66fbb251b5803b3972be99157
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("membershipRuleProcessingState eq 'On'")
    .Select("id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus")
    .GetAsync();

```