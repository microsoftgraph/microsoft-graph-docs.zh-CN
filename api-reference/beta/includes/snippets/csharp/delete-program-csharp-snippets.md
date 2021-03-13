---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f922d877fc0009b1e3b99fb1e0399d1ff191b928
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Programs["{program-id}"]
    .Request()
    .DeleteAsync();

```