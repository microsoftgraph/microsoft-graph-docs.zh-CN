---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b30ede5875ff2e10b3d9bf4dbe29345211243e5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domainNameReferences = await graphClient.Domains["contoso.com"].DomainNameReferences
    .Request()
    .GetAsync();

```