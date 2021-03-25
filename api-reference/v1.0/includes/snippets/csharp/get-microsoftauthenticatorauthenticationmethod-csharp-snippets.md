---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 585d256f2145dc795953a2c8dc9d522f629f02ca
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftAuthenticatorAuthenticationMethod = await graphClient.Users["{user-id}"].Authentication.MicrosoftAuthenticatorMethods["{microsoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```