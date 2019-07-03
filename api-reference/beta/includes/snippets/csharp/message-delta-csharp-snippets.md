---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f34e97d12099d0cd49a53787b6877f507790f8e3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478919"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders["{id}"].Messages.Delta()
    .Request()
    .GetAsync();

```