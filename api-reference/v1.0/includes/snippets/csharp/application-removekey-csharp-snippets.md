---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09ca117c68ebd9ac9da59e450c89d60c3501cb93
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

var proof = "eyJ0eXAiOiJ...";

await graphClient.Applications["{id}"]
    .RemoveKey(keyId,proof)
    .Request()
    .PostAsync();

```