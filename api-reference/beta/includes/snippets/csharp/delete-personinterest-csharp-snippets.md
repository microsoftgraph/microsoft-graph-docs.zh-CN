---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19b5a9b260f955b6acd3277afbf20f3ee431490d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Interests["{personInterest-id}"]
    .Request()
    .DeleteAsync();

```