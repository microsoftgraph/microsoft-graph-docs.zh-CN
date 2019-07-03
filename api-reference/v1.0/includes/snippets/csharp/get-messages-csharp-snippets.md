---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ca5b571dad3993a594da8b1197e4437174a38d76
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Select( e => new {
             e.Sender,
             e.Subject 
             })
    .GetAsync();

```