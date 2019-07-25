---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c72fc0fec734d1b65578dfe25b13794355ba9c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.MobilePhone 
             })
    .GetAsync();

```