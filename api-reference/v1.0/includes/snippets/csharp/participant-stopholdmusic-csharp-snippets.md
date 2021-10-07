---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6efcd062354556c9b1d937b8672ccc04994a66f0
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214620"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .StopHoldMusic(clientContext)
    .Request()
    .PostAsync();

```