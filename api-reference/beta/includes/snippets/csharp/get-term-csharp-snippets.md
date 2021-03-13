---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c4d66f63449f4191093ca547bb1c98524b5ad44
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = await graphClient.TermStore.Groups["{termStore.group-id}"].Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .GetAsync();

```