---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f324309b5795c36acda4f59f4c435aaf1d4cd380
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","microsoft.graph.mailSearchFolder"}
    },
    FilterQuery = "contains(subject, 'Analytics')"
};

await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .UpdateAsync(mailFolder);

```