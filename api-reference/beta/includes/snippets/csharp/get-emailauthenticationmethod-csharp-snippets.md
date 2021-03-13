---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87ee18f076cf9e705ddf997653ca134ae8b08f2f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = await graphClient.Me.Authentication.EmailMethods["{emailAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```