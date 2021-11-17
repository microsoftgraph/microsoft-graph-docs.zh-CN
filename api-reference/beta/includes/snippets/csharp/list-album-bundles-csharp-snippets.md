---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cce3b217731bba14acbdb2966c25417b66e75dc4a1891ca23bc8f083e2e39c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162298"
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