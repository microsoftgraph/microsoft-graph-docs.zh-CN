---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0948b00d09234f10da6195edbe21d7b64d9a36ee
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609152"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["searchfolders"].ChildFolders
    .Request()
    .GetAsync();

```