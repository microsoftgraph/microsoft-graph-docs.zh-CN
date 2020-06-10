---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a27130770eb1291d67d18c6435906b3cc5a44ad4
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var requests = new List<SearchRequestObject>()
{
    new SearchRequestObject
    {
        EntityTypes = new List<EntityType>()
        {
            EntityType.ExternalItem
        },
        ContentSources = new List<String>()
        {
            "/external/connections/connectionfriendlyname"
        },
        Query = new SearchQuery
        {
            Query_string = new SearchQueryString
            {
                Query = "contoso product"
            }
        },
        From = 0,
        Size = 25,
        Stored_fields = new List<String>()
        {
            "title",
            "description"
        }
    }
};

await graphClient.Search
    .Query(requests)
    .Request()
    .PostAsync();

```