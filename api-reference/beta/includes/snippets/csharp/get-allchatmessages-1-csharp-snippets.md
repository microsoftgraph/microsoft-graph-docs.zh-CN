---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 168e5bbb5f9fd73607e7905e0b6e53579df85f68
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100543"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .OrderBy("createdDateTime")
    .Top(2)
    .GetAsync();

```