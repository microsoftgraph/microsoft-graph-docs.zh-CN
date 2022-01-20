---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf5eeb22252f00af59d300050110917f612d922d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .Renew()
    .Request()
    .PostAsync();

```