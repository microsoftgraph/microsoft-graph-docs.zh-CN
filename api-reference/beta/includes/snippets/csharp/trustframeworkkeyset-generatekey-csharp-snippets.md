---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc073e4ff9b04696c1086d827a310ad0598b08caf1ce7cec4992c0d6f3fa5bfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277738"
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