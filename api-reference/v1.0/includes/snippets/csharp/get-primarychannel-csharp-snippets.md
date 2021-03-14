---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c54b977153c8564cf33f306815306f9375a6b29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{team-id}"].PrimaryChannel
    .Request()
    .GetAsync();

```