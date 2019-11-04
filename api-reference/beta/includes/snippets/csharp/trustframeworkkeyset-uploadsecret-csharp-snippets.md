---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b3393a66c199e75a0744d77e14064768a5a3f67
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var use = "use-value";

var k = "application-secret-to-be-uploaded";

var nbf = 1508969811;

var exp = 1508973711;

await graphClient.TrustFramework.KeySets["{id}"]
    .UploadSecret(use,k,nbf,exp)
    .Request()
    .PostAsync();

```