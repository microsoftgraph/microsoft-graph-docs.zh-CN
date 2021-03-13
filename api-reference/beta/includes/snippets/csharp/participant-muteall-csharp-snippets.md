---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a652b126f1e96fe1bd5eeba3e4e2e654242d302
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<String>()
{
    ""
};

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"].Participants
    .MuteAll(participants,clientContext)
    .Request()
    .PostAsync();

```