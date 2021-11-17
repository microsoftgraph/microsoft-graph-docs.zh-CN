---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 972967a1ea1c7d88a2a061950d2a143422cea3700951318457d85c0939945347
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("forcedelete", "true")
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags["{ediscovery.tag-id}"]
    .Request( queryOptions )
    .DeleteAsync();

```