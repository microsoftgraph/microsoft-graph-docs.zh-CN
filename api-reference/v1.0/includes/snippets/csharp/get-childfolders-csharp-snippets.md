---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 225977cd90be1c813c8489792b21b01d95008e5b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["{id}"].ChildFolders
    .Request()
    .GetAsync();

```