---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c043db41b5ad9a003f0dd54bff391664f792eea256ccec08b089103a8000a26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"]
    .Request()
    .GetAsync();

```