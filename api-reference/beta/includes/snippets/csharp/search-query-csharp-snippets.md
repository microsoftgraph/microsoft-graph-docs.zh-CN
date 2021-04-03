---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7042865916b90ae7b34c117b652601266f464cb9
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573148"
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