---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f1cd9bcc652659b1e8ba2bdd3b3ef61baf6e6b5f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.GivenName,
             e.PostalCode 
             })
    .GetAsync();

```