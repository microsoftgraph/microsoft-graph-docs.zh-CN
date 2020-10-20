---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da3483616be48434ac83dc126a7bdda639dc5205
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.ServicePrincipals["{id}"]
    .Request()
    .GetAsync();

```