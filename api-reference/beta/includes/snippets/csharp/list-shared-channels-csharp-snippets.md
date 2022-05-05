---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e842ea59025064771362b052e73c4d7f92d977c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{team-id}"].Channels
    .Request()
    .Filter("membershipType eq 'shared'")
    .GetAsync();

```