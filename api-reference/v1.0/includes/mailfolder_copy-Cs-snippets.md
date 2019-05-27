---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f3980b66f62545f5dc7f920ed33699d31677c93
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```