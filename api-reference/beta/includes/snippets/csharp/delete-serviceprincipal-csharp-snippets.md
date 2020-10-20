---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f879328da6bf2fda942721a62d571e879a794d2e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"]
    .Request()
    .DeleteAsync();

```