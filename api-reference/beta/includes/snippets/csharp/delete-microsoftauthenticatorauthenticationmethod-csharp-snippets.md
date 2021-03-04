---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4be7d125740caede751f430570f2cee6baa428b8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["kim@contoso.com"].Authentication.MicrosoftAuthenticatorMethods["_jpuR-TGZtk6aQCLF3BQjA2"]
    .Request()
    .DeleteAsync();

```