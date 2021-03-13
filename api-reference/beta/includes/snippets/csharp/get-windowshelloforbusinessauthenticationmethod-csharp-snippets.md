---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97854a0a62182f2c6f60aad269c8723beccd0255
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788401"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsHelloForBusinessAuthenticationMethod = await graphClient.Users["{user-id}"].Authentication.WindowsHelloForBusinessMethods["{windowsHelloForBusinessAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```