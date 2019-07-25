---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 988379b0f1f73bbff16c66dc5df4999258d89eb0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolders = await graphClient.Me.MailFolders
    .Request()
    .GetAsync();

```