---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75f045078b8ace76d578e94dc5fc37ffa3bf840a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Owners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```