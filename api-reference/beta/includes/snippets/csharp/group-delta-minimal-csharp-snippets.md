---
description: 自动生成的文件。 不修改
ms.openlocfilehash: df92fbd764efbe2ac853ad4236e5cd08c23a8c12
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858751"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Groups
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select( e => new {
             e.DisplayName,
             e.Description,
             e.MailNickname 
             })
    .GetAsync();

```