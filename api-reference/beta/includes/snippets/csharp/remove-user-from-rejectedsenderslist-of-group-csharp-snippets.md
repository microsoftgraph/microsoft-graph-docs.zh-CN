---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b476cef65edcf406c1be7d8a1030197970d59349
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].RejectedSenders.References
    .Request()
    .DeleteAsync();

```