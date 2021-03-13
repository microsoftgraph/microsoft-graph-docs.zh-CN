---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21c3d2bbcd1f351c7fb8c84f9c9832a77d49423a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803307"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54";

await graphClient.Communications.Calls["{call-id}"]
    .SubscribeToTone(clientContext)
    .Request()
    .PostAsync();

```