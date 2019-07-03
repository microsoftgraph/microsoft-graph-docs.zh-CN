---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f4857e5e52c2cb2f27cff8dbc7438e4884a3b6f0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADhAAAW-VPeAAA="]
    .Request()
    .Select( e => new {
             e.InternetMessageHeaders 
             })
    .GetAsync();

```