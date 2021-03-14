---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f3011688b99398e9700d5fec07339892d55e6bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .DeleteAsync();

```