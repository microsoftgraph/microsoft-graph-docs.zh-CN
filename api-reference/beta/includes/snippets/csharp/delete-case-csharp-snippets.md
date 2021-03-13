---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80a8572c97018a7aee4ff1264df12d6b3332f19c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Request()
    .DeleteAsync();

```