---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2a5841750923854639aad96c942906f2fd5456d
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757890"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("filter", "bundle/album ne null")
};

var bundles = await graphClient.Drive.Bundles
    .Request( queryOptions )
    .Filter("bundle/album ne null")
    .GetAsync();

```