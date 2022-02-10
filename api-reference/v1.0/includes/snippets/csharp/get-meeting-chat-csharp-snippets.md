---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a272c0c67834c05aa4f764088269f2f52ad1e61
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Chats["{chat-id}"]
    .Request()
    .GetAsync();

```