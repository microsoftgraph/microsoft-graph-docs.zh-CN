---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 47878de99bfd6c4577bd16aa49976be075a5bf00
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729681"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .UpdateAsync(mailFolder);

```