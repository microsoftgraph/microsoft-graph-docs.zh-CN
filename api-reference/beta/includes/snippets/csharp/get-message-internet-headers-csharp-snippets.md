---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 04610788acf8d158a15e4d1a1d0fb3516046dd13
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520315"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGVmMDEz"]
    .Request()
    .Select( e => new {
             e.InternetMessageHeaders 
             })
    .GetAsync();

```