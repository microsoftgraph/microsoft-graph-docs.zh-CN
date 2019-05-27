---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2ef5bd45ac194d6bd9c147e0bbba28cfb8b1d80e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders.Delta()
    .Request()
    .GetAsync();

```