---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e1d8527950a0c35cee1dcbd3c95bae373e94666
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788411"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-id}"]
    .Verify()
    .Request()
    .PostAsync();

```