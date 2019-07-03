---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d73dbe112c680a3e3fa0a5ea0c69ad0e46aae649
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509246"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{id}"]
    .Move(destinationId)
    .Request()
    .PostAsync();

```