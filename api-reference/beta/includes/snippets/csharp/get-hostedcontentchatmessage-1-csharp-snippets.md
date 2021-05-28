---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b481c42846b6460de1ffceebdc35ae7dcff2a96
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessageHostedContent = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents["{chatMessageHostedContent-id}"]
    .Request()
    .GetAsync();

```