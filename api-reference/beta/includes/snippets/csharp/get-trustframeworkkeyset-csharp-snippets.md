---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b23ea64743b33498260d31edc62d755ca3dd3fa9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trustFrameworkKeySet = await graphClient.TrustFramework.KeySets["{id}"]
    .Request()
    .GetAsync();

```