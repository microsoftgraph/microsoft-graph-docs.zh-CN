---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54b104649dc0caa53412b07f321a009d45a3ef6c
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "Clutter",
    IsHidden = true
};

await graphClient.Me.MailFolders
    .Request()
    .AddAsync(mailFolder);

```