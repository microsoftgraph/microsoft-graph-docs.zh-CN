---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 080cfe2d99655b51a73b96a70c6b77854976ad0c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Chats["{chat-id}"].Members
    .Request()
    .GetAsync();

```