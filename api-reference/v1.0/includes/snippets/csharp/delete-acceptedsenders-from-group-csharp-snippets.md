---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 345e8e8a963201a31169aaade284bcbf16ab4afa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].AcceptedSenders.References
    .Request()
    .DeleteAsync();

```