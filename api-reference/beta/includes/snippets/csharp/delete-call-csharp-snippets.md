---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80311ccb656ae9901418312ee2011d5a62d9905e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783885"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"]
    .Request()
    .DeleteAsync();

```