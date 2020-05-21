---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f012126064b6edd912164fcface786c4de93020a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334885"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

var proof = "eyJ0eXAiOiJ...";

await graphClient.Serviceprincipals["{id}"]
    .RemoveKey(keyId,proof)
    .Request()
    .PostAsync();

```