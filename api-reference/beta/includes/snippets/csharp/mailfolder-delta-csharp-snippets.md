---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2ef5bd45ac194d6bd9c147e0bbba28cfb8b1d80e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders.Delta()
    .Request()
    .GetAsync();

```