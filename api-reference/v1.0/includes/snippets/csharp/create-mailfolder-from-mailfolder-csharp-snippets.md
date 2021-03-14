---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc94bb69ce4bf814b566d9e7994b0ee45f1047a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```