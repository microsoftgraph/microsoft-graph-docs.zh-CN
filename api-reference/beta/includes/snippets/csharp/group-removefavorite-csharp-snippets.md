---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9241ef7b16f259f39e00de16b8c86f00eb499b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779243"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .RemoveFavorite()
    .Request()
    .PostAsync();

```