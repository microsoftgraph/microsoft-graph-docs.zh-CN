---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9a9dbc1c12e3193dfdb47686d36aef70d4044b87867af49ee23313467105395
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215926"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodsPolicy = await graphClient.Policies.AuthenticationMethodsPolicy
    .Request()
    .GetAsync();

```