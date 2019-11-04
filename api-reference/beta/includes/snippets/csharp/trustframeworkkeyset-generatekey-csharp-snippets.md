---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3933b32ffd201e96edbfca63f1f76f4dd07f4215
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var use = "sig";

var kty = "RSA";

var nbf = 1508969811;

var exp = 1508969811;

await graphClient.TrustFramework.KeySets["{id}"]
    .GenerateKey(use,kty,nbf,exp)
    .Request()
    .PostAsync();

```