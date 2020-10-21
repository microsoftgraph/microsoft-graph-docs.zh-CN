---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da0ac949daf734cac5f1a82d85e5b77bd736f0a8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621580"
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