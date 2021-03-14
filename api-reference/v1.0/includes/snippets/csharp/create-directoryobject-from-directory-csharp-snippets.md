---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e65a98e28b36ce07a4b460437867623bed3b2160
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{directoryObject-id}"]
    .Restore()
    .Request()
    .PostAsync();

```