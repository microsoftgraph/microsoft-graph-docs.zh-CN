---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c8496341efb44efb0a4304c4ae6dfec99549f75
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Notebooks["{id}"]
    .CopyNotebook(groupId,renameAs,null,null,null)
    .Request()
    .PostAsync();

```