---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30ed1c7a856b6aef5fc3f7d1cf02ed6dc2579e20
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .AddFavorite()
    .Request()
    .PostAsync();

```