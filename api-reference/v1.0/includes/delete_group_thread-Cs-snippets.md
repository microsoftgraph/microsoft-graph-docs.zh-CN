---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 33741f0082e92bd20c0e8dbc25278f758674a5b1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].Threads["AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="]
    .Request()
    .DeleteAsync();

```