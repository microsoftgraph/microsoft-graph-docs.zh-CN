---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09751c0a4bfcaa1a76059f149d79adbb1bbbadf4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796570"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var use = "sig";

var kty = "RSA";

var nbf = 1508969811;

var exp = 1508969811;

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .GenerateKey(use,kty,nbf,exp)
    .Request()
    .PostAsync();

```