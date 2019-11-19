---
title: 搜索文件（包括 externalFile）
description: 查询 API 允许您跨文件搜索（DriveItem 或外部文件）。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 95a8b99b9970ec239935ee2c35afeec581a1b35f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703945"
---
# <a name="search-files-including-externalfile"></a>搜索文件（包括 externalFile）

Microsoft Search API 允许你搜索存储在 SharePoint 或 OneDrive 中的文件。 它使用相关性模型，该模型利用来自 Microsoft Graph 的有关用户的关系和活动的信号。 这样，就可以在与 SharePoint 中列出搜索结果的 "**文件**" 选项卡一致的文件搜索体验中，返回和提升用户关注的内容。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

此外，API 还可以通过[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta)资源公开公开外部文件。

## <a name="search-sharepoint-or-onedrive-files"></a>搜索 SharePoint 或 OneDrive 文件

您可以在 SharePoint 和 OneDrive 查询的搜索词中使用 KQL。 例如：

- `"query" : "contoso filetype:docx OR filetype:doc"`将查询范围限定为 Word 文档
- `"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`将查询范围限定为网站中的特定文件夹。

属性限制必须在条件中指定有效的可查询托管属性名称，这样才能有效。

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

下面是一个响应示例。

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

[文件共享连接器](/MicrosoftSearch/file-share-connector)是 Microsoft Search 中可用的 "开箱即用" 连接器。 它使您能够索引文件共享上可用的文件。 您可以使用查询 API 查询所有外部文件。

<!-- markdownlint-disable MD024 -->
### <a name="example"></a>示例

下面的示例返回租户的所有已配置的 externalFile 连接器，并按相关性对结果进行排序。

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

您可以通过在搜索请求中指定两个实体类型来搜索租户中的所有文件，包括[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)和所有外部文件。

响应在每个[searchHit](/graph/api/resources/searchhit?view=graph-rest-beta)对象**** 的`_sources`字段中提供了 driveItem 和 externalItem 实例的组合。

### <a name="example"></a>示例

下面的示例返回满足搜索词的租户的所有配置的**externalFile**连接器和**driveItem**对象。 它按相关性对结果进行排序。

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

无法将查询限定为特定 connectionId。

## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [使用搜索 API](/graph/api/resources/search-api-overview?view=graph-rest-beta)
