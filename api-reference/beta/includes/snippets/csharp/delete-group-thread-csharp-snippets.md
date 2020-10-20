---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33741f0082e92bd20c0e8dbc25278f758674a5b1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].Threads["AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="]
    .Request()
    .DeleteAsync();

```