---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7707fa1aacc8d59f0fee5c8eeb3dce7a2257c8c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var key = "key-value";

await graphClient.TrustFramework.KeySets["{id}"]
    .UploadCertificate(key)
    .Request()
    .PostAsync();

```