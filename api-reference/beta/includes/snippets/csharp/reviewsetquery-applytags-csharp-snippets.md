---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b192d9e53b6fc7e1cf9dd0dfd1db7840ea31fd8941f929e851f39f791a5442e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tagsToAdd = new List<Microsoft.Graph.Ediscovery.Tag>()
{
    new Microsoft.Graph.Ediscovery.Tag
    {
        Id = "b4798d14-748d-468e-a1ec-96a2b1d49677"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"].Queries["{ediscovery.reviewSetQuery-id}"]
    .ApplyTags(tagsToAdd,null)
    .Request()
    .PostAsync();

```