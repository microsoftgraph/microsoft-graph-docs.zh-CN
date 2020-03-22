---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索文件
description: 您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: a75eb8e90c8656ced3d9f50d6526b5ebe48584aa
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892672"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a>在 Microsoft Graph 中使用 Microsoft Search API 搜索文件

您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。 Microsoft Search API 使用相关性模型，该模型利用来自 Microsoft Graph 的有关用户的关系和活动的信号。 这使您能够在与 SharePoint 中列出搜索结果**的文件选项卡一致**的文件搜索体验中返回和提升用户关注的内容。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="search-sharepoint-or-onedrive-files"></a>搜索 SharePoint 或 OneDrive 文件

您可以在 SharePoint 和 OneDrive 查询的搜索词中使用 KQL。 例如：

- `"query": "contoso filetype:docx OR filetype:doc"`将查询范围限定为 Word 文档。
- `"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`将查询范围限定为网站中的特定文件夹。

属性限制必须在条件中指定有效且可查询的托管属性名称，这样才能有效。

### <a name="example"></a>示例

#### <a name="request"></a>请求

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a>响应

<!---TODO nmoreau team Include one example of externalItem response.-->
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "test"
      ],
      "hitsContainers": [
        {
          "total": 350,
          "moreResultsAvailable": true,
          "hits": [
            {
              "_id": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "_score": 1,
              "_sortField": "Relevance",
              "_summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "_source": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "fileSystemInfo": {
                  "createdDateTime": "2019-06-10T06:37:43Z",
                  "lastModifiedDateTime": "2019-06-10T06:37:43Z"
                }
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta)
