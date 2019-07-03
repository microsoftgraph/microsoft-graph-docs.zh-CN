---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0948b00d09234f10da6195edbe21d7b64d9a36ee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["searchfolders"].ChildFolders
    .Request()
    .GetAsync();

```