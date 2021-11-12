---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f7cf0ee6b0739ab741b8f9e72151c13a9830316ce33c8be437bf36af240fca1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailSearchFolder
{
    DisplayName = "Weekly digests",
    IncludeNestedFolders = true,
    SourceFolderIds = new List<String>()
    {
        "AQMkADYAAAIBDAAAAA=="
    },
    FilterQuery = "contains(subject, 'weekly digest')"
};

await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```