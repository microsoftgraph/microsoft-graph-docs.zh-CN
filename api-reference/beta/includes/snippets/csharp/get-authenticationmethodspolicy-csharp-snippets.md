---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16e414a7f3a31cb3e0f8f0da97760a3789e55a05
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodsPolicy = await graphClient.Policies.AuthenticationMethodsPolicy
    .Request()
    .GetAsync();

```