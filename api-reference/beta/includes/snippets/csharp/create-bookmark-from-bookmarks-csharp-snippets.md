---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fdb1b0a1b7b792be5a25a8a95b415547709105a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookmark = new Microsoft.Graph.Search.Bookmark
{
    DisplayName = "Contoso Install Site",
    WebUrl = "http://www.contoso.com/",
    Description = "Try or buy Contoso for Home or Business and view product information",
    Keywords = new Microsoft.Graph.Search.AnswerKeyword
    {
        Keywords = new List<String>()
        {
            "Contoso",
            "install"
        },
        ReservedKeywords = new List<String>()
        {
            "Contoso"
        },
        MatchSimilarKeywords = true
    },
    AvailabilityStartDateTime = null,
    AvailabilityEndDateTime = null,
    Platforms = new List<DevicePlatformType>()
    {
        DevicePlatformType.Android
    },
    TargetedVariations = new List<Microsoft.Graph.Search.AnswerVariant>()
    {
        new Microsoft.Graph.Search.AnswerVariant
        {
            LanguageTag = "es-ES",
            DisplayName = "Sitio de instalación Contoso",
            Description = "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
        }
    },
    GroupIds = new List<String>()
    {
        "groupId"
    },
    PowerAppIds = new List<String>()
    {
        "powerAppId"
    },
    State = Microsoft.Graph.Search.AnswerState.Published
};

await graphClient.Search.Bookmarks
    .Request()
    .AddAsync(bookmark);

```