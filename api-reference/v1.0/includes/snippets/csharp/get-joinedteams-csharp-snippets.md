---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45fe4fca4cb73b1f59e3054a18cb679cb8da80e789f02ba720de13e21c1e3f65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164124"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var joinedTeams = await graphClient.Me.JoinedTeams
    .Request()
    .GetAsync();

```