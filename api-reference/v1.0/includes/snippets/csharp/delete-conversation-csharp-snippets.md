---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd14a5c71fd91f258bb6532209bc502c29225e03
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"]
    .Request()
    .DeleteAsync();

```