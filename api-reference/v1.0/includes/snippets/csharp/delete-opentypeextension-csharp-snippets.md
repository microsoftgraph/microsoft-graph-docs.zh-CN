---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cc0add875b4e630bd807ec054f12ebecde0fdd8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788444"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"].Extensions["{extension-id}"]
    .Request()
    .DeleteAsync();

```