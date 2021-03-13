---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 790ed6a35f5212c3506b03605447af53bed36ce0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .AddCopy(contentType)
    .Request()
    .PostAsync();

```