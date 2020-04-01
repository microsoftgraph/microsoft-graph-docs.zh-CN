---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 259d243bb8e6054b59c0034bebf21b6dee915597
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["delta"]
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.Mail 
             })
    .GetAsync();

```