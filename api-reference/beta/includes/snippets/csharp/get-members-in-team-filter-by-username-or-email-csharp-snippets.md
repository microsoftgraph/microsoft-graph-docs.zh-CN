---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3700ad9e87869299d437575edbc54c80fd1b6f7f
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062"].Members
    .Request()
    .Filter("(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')")
    .GetAsync();

```