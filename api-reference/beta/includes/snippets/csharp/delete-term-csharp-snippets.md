---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d1e59bdd9eefe53be5049c1e01cadfed3c8c579
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .DeleteAsync();

```