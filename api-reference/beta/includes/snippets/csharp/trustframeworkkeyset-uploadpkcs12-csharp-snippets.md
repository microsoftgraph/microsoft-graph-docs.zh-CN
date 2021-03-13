---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da4cd5c54a862b4c6853b0708dfb12054898a0bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var key = "Base64-encoded-pfx-content";

var password = "password-value";

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .UploadPkcs12(key,password)
    .Request()
    .PostAsync();

```