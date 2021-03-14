---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c6d10926ef59711a7bcd51dd92618168b79c8e8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787036"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members["{conversationMember-id}"]
    .Request()
    .GetAsync();

```