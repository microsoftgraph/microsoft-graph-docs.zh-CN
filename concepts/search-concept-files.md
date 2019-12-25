---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索文件
description: 您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0b8db24a8b9ccd63ac3d3be800b209a64eb3aa9d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866915"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a>在 Microsoft Graph 中使用 Microsoft Search API 搜索文件

您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。 Microsoft Search API 使用相关性模型，该模型利用来自 Microsoft Graph 的有关用户的关系和活动的信号。 这使您能够在与 SharePoint 中列出搜索结果**的文件选项卡一致**的文件搜索体验中返回和提升用户关注的内容。 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

API 还可以通过[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta)资源公开公开的外部文件。

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

## <a name="search-external-files-well-known-types"></a>搜索外部文件（已知类型）

默认情况下，[文件共享连接器](/MicrosoftSearch/file-share-connector)在 Microsoft Search 中可用。 您可以使用它来索引文件共享上可用的文件。 您可以使用查询 API 查询所有外部文件。

<!-- markdownlint-disable MD024 -->
### <a name="example"></a>示例

下面的示例返回租户的所有已配置的外部文件，并按相关性对结果进行排序。

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
        "microsoft.graph.externalFile"
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

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 4,
          "moreResultsAvailable": true,
          // Hits represent the search results
          "hits": [
            {
              "_id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
              "_score": 1,
              "_sortField": "Relevance",
              "_source": {
                "@odata.type": "#microsoft.graph.externalFile",
                "id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
                "extension": "pptx",
                "name": "Contoso-Overview.pptx",
                "lastModifiedTime": "2018-05-09T04:01:14Z",
                "modifiedBy": "Baala Vedantam",
                "title": "Contoso Overview 2018",
                "url": "file://fileshare01/External Presentations/Contoso-Overview.pptx"
              }
            },
            {
              //Another searchHit
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="search-all-files-including-externalfile-instances"></a>搜索所有文件（包括 externalFile 实例）

您可以通过在搜索请求中指定两个实体类型来搜索租户中的所有文件，包括存储在[driveitem](/graph/api/resources/driveitem?view=graph-rest-beta)和外部文件中的文件。

响应包括每个[searchHit](/graph/api/resources/searchhit?view=graph-rest-beta)对象的`_sources`字段中的**driveItem**和**externalItem**实例。

### <a name="example"></a>示例

下面的示例返回租户中满足搜索词的所有已配置的**externalFile**和**driveItem**对象。 它按相关性对结果进行排序。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem",
        "microsoft.graph.externalFile"
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

## <a name="known-limitations"></a>已知限制

无法将查询限定为特定的连接 ID。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta)

