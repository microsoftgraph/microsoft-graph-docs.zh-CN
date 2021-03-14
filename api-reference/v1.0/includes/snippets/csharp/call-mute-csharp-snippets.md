---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09525ded5816363210b54ade2daa7cdf5813f72a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```