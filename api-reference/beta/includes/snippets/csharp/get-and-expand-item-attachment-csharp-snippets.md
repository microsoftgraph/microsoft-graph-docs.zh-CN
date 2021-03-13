---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b8b37e1e18037ecc02642d2d5264447282311aa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["{message-id}"].Attachments["{attachment-id}"]
    .Request()
    .Expand("itemattachment/item")
    .GetAsync();

```