---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34934642fe8487de39095f48a936c332f84eacf94e22a015cdefbf2a336af1bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .ProvisionEmail()
    .Request()
    .PostAsync();

```