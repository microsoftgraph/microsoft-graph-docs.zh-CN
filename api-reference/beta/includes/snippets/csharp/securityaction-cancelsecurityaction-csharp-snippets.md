---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc16651da064cc8bc9ca85050ecf62cb06033c47
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.SecurityActions["{securityAction-id}"]
    .CancelSecurityAction()
    .Request()
    .PostAsync();

```