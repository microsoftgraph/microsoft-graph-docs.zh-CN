---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e70499a6f256dfb5acd09e5e3d198851af6a49ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```