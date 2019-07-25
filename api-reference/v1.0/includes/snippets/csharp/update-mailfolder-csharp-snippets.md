---
description: 自动生成的文件。 不修改
ms.openlocfilehash: da0ac949daf734cac5f1a82d85e5b77bd736f0a8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders["{id}"]
    .Request()
    .UpdateAsync(mailFolder);

```