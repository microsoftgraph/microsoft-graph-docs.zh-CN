---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 06f7aab4f4e38d8a2fda4a6a5bc22e807b4826d7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders["{id}"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```