---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ee8d79446c5bbaaa6d5ae1d2e0f10a5e5f9ea0acff1edda5942ec8d2ade235e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277389"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Users["{user-id}"].UsageRights
    .Request()
    .GetAsync();

```