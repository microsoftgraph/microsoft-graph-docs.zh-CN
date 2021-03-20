---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd3b8f47d8f6d12d288f8eacddacebf8fc95afd6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var history = await graphClient.IdentityProtection.RiskyUsers["{riskyUser-id}"].History
    .Request()
    .GetAsync();

```