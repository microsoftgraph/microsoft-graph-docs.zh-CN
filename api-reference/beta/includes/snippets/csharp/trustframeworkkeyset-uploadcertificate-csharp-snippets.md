---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 910358da013f57cd9006291ca227fde500fac1e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810101"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var key = "key-value";

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .UploadCertificate(key)
    .Request()
    .PostAsync();

```