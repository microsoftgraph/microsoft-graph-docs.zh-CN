---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcb3eb3e251157ab20d2caf5e16cbe0006be6868
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```