---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 168b72816bfbb8b39208e8173edeb7fc61d1a6c63aef42703579cc19b2f6c63d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218896"
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
            QueryString = "contoso product"
        },
        From = 0,
        Size = 25,
        Fields = new List<String>()
        {
            "title",
            "description"
        }
    }
};

await graphClient.Search
    .Query(requests,null)
    .Request()
    .PostAsync();

```