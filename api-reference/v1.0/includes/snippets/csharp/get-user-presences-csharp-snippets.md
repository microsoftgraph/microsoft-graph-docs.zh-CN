---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7041d60aeb76042d736358124ed400d704157863
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Communications.Presences["{presence-id}"]
    .Request()
    .GetAsync();

```