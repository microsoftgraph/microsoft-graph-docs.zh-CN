---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1508732d9470e4cc5d1118c22565fc951ba42304839f520565d6a52ec8f3be13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107131"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sitePage = new SitePage
{
    Name = "Events.aspx",
    Title = "Team Events",
    PublishingState = new PublicationFacet
    {
        Level = "checkedOut",
        VersionId = "0.1"
    },
    WebParts = new List<WebPart>()
    {
        new WebPart
        {
            Type = "rte",
            Data = new SitePageData
            {
                AdditionalData = new Dictionary<string, object>()
                {
                    {"innerHTML", "<p>Here are the team's upcoming events:</p>"}
                }
            }
        },
        new WebPart
        {
            Type = "d1d91016-032f-456d-98a4-721247c305e8",
            Data = new SitePageData
            {
                AdditionalData = new Dictionary<string, object>()
                {
                    {"title", "Events"},
                    {"description", "Display upcoming events"},
                    {"serverProcessedContent", "{\"htmlStrings\":{},\"searchablePlainTexts\":{\"title\":\"\"},\"imageSources\":{},\"links\":{\"baseUrl\":\"https://www.contoso.com/sites/Engineering\"},\"componentDependencies\":{\"layoutComponentId\":\"8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027\"}}"},
                    {"dataVersion", "1.0"},
                    {"properties", "{\"selectedListId\":\"032e08ab-89b0-4d8f-bc10-73094233615c\",\"selectedCategory\":\"\",\"dateRangeOption\":0,\"startDate\":\"\",\"endDate\":\"\",\"isOnSeeAllPage\":false,\"layoutId\":\"FilmStrip\",\"dataProviderId\":\"Event\",\"webId\":\"0764c419-1ecc-4126-ba32-0c25ae0fffe8\",\"siteId\":\"6b4ffc7a-cfc2-4a76-903a-1cc3686dee23\"}"}
                }
            }
        }
    }
};

await graphClient.Sites["{site-id}"].Pages
    .Request()
    .AddAsync(sitePage);

```