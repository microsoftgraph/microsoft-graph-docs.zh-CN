---
title: 为打印机创建 printJob
description: 为打印机创建新的 printJob。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9298682cd33509f1ffb6beaa850fbd33a761b42c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855761"
---
# <a name="create-printjob-for-a-printer"></a>为打印机创建 printJob

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为[打印机](../resources/printer.md)创建新的 [printJob](../resources/printJob.md)。 

> **注意：** 用户可以在 10 天内提交最多 10000 个打印作业。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [Get 打印机](printer-get.md) 访问权限的权限。 已登录的用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob.Create、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |
| Content-type  | application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [printJob](../resources/printjob.md) 对象的 JSON 表示形式。 printJob 对象应仅包含 **配置**。 **配置** 的所有属性都是可以为 null 的。 在创建资源期间会自动设置所有其他字段，包括作业和文档 ID。

目前，通用打印仅支持每个 **printJob** 对象一个 **printDocument**。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [printJob](../resources/printjob.md) 对象以及关联的 [printDocument](../resources/printDocument.md) 。 
## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob_1"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
Content-type: application/json

{
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
  "id": "1825",
  "createdDateTime": "2020-10-14T05:16:49-07:00",
  "isFetchable": false,
  "redirectedFrom": null,
  "redirectedTo": null,
  "createdBy": {
    "id": "{userId}",
    "displayName": "{username}",
    "ipAddress": null,
    "userPrincipalName": "{userupn}"
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet.",
    "isAcquiredByPrinter": false,
    "details": [
      "uploadPending"
    ]
  },
  "configuration": {
    "quality": "medium",
    "dpi": 600,
    "feedOrientation": "longEdgeFirst",
    "orientation": "landscape",
    "duplexMode": "oneSided",
    "copies": 1,
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false,
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    }
  },
  "documents": [
    {
      "id": "1477576d-5dab-4ea9-865c-c0b82cd70bd5",
      "displayName": "",
      "contentType": "",
      "size": 0
    }
  ]
}
```
