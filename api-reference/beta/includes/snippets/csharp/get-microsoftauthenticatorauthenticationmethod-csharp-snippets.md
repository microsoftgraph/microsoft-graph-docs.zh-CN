---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39a1f923137a19a897e66030312f94ed1dda47eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftAuthenticatorAuthenticationMethod = await graphClient.Users["anirban@contoso.com"].Authentication.MicrosoftAuthenticatorMethods["_jpuR-TGZtk6aQCLF3BQjA2"]
    .Request()
    .GetAsync();

```