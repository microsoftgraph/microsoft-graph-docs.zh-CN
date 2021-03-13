---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 816bba87da678a8601a6baf992354d16ff81d2e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tag = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags["{ediscovery.tag-id}"]
    .Request()
    .GetAsync();

```