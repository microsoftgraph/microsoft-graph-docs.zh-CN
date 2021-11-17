---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 610dfd44d7fb4715eab8ef8022ac6c69b30797250fba51df120ba014f836abbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

var membershipRule = "(user.displayName -startsWith \"EndTestUser\")";

await graphClient.Groups
    .EvaluateDynamicMembership(memberId,membershipRule)
    .Request()
    .PostAsync();

```