---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50368980e58015c5139f657c6cc6e748d0da34729710e912f04573ef2c7a4310
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents["{chatMessageHostedContent-id}"].Content
    .Request()
    .GetAsync();

```