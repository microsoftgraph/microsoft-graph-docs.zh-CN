---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d73dbe112c680a3e3fa0a5ea0c69ad0e46aae649
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721622"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{id}"]
    .Move(destinationId)
    .Request()
    .PostAsync();

```