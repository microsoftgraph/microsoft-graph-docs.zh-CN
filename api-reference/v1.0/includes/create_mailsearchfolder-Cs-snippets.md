---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea6cb94b3c7204233c7387058ef4da371631d434
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "Weekly digests",
    IncludeNestedFolders = true,
    SourceFolderIds = new List<String>()
    {
        "AQMkADYAAAIBDAAAAA=="
    },
    FilterQuery = "contains(subject, 'weekly digest')"
};

await graphClient.Me.MailFolders["AQMkADYAAAIBDAAAAA=="].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```