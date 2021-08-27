---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 611f3d19841302ce3f915c01d4e084c13f559b224436cf35ebbf1adebbc8d3e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .GetAsync();

```