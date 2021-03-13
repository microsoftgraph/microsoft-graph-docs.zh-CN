---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d031d0b80fae525134e0fc2ac7956513cb5f99c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Move(destinationId)
    .Request()
    .PostAsync();

```