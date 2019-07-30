---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a2a5841750923854639aad96c942906f2fd5456d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932655"
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