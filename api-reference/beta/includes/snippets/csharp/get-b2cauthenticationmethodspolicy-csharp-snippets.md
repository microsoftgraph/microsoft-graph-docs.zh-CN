---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 442d2e6328b3e448a005a46add56e6ebe686c54ed208a3b86336ef9672abae72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cAuthenticationMethodsPolicy = await graphClient.Policies.B2cAuthenticationMethodsPolicy
    .Request()
    .GetAsync();

```