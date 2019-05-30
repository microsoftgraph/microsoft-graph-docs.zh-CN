---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fbeeae776efbea0ae1aab65c9719e4177862c5a5
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "Get MyAnalytics",
    IncludeNestedFolders = true,
    SourceFolderIDs = new List<String>()
    {
        "AAMkAGVmMDEzM"
    },
    FilterQuery = "contains(subject, 'MyAnalytics')"
};

await graphClient.Me.MailFolders["searchfolders"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```