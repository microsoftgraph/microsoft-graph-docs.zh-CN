---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 898aa716726ec5e2438136b0d31954ae5216f4ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Sections["{onenoteSection-id}"]
    .CopyToNotebook(id,groupId,renameAs,null,null)
    .Request()
    .PostAsync();

```