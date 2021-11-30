---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3def0628d12992a5d90fa260c11a5262b672a138
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .Select("customSecurityAttributes")
    .GetAsync();

```