---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be243e365a50867db2569a987ff62ea495d547dd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new AuthenticationMethodConfiguration
{
    IsUsableOnce = true
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```