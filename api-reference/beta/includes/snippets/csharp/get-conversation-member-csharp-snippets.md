---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad887bcf9626c36fe2907e8b87c8bdf20e3c6678
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633305"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Chats["{id}"].Members["{id}"]
    .Request()
    .GetAsync();

```