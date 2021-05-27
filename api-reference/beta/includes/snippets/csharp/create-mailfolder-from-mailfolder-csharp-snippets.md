---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2578f655fd49ba55d4c93ae96d15abb10cd6522
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668712"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value",
    IsHidden = true
};

await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```