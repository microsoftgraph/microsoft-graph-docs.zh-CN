---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5587acf5f6bf337baf1a6011089c4511fa5c385
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731308"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["{id}"]
    .Request()
    .DeleteAsync();

```