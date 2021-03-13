---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e16307e33185fd2bacca0b25bc35949ba7a65cb7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tags = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags
    .Request()
    .GetAsync();

```