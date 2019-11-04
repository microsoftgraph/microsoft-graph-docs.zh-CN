---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dae24769a0cdf6dcfa76558803dbc6cbafdfc669
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var key = "Base64-encoded-pfx-content";

var password = "password-value";

await graphClient.TrustFramework.KeySets["{id}"]
    .UploadPkcs12(key,password)
    .Request()
    .PostAsync();

```