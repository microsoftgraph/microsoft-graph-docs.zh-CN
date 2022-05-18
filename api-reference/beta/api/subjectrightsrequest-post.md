---
title: 创建 subjectRightsRequest
description: 创建新的 subjectRightsRequest 对象。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9c4530948142d639295993d24f4c44392e647af4
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461490"
---
# <a name="create-subjectrightsrequest"></a>创建 subjectRightsRequest
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [subjectRightsRequest](../resources/subjectrightsrequest.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|SubjectRightsRequest.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持|

## <a name="http-request"></a>HTTP 请求

[!INCLUDE [subject-rights-request-privacy-deprecate](../../includes/subject-rights-request-privacy-deprecate.md)]

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/subjectRightsRequests
POST /privacy/subjectRightsRequests

```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [subjectRightsRequest](../resources/subjectrightsrequest.md) 对象的 JSON 表示形式。

下表显示了创建 [subjectRightsRequest](../resources/subjectrightsrequest.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
| contentQuery         | String | KQL应用于搜索的内容查询。 此属性仅针对使用 `\security` 查询路径而不是查询路径 `\privacy` 访问的 API 定义。|
|dataSubject|[microsoft.graph.dataSubject](../resources/datasubject.md)|包含请求的数据主体的属性。|
|dataSubjectType|dataSubjectType|数据主体类型。 可取值为：`customer`、`currentEmployee`、`formerEmployee`、`prospectiveEmployee`、`student`、`teacher`、`faculty`、`other`、`unknownFutureValue`。|
|说明|字符串|请求的说明。|
|displayName|String|请求的名称。|
| externalId           | String| 创建后不可变的请求的外部 ID，用于跟踪外部系统的请求。 此属性仅针对使用 `\security` 查询路径而不是查询路径 `\privacy` 访问的 API 定义。|
| includeAllVersions   | 布尔值 | 包括文档的所有版本。 默认情况下，将返回文档的当前副本。 如果SharePoint站点已启用版本控制，包括所有版本将包括文档的历史副本。 此属性仅针对使用 `\security` 查询路径而不是查询路径 `\privacy` 访问的 API 定义。|
| includeAuthoredContent| 布尔值 | 包括由数据主体创作的内容。 此属性仅针对使用 `\security` 查询路径而不是查询路径 `\privacy` 访问的 API 定义。|
|internalDueDateTime|DateTimeOffset|用于跟踪请求完成的内部截止日期。|
| mailboxLocations     | [subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md)|应搜索的邮箱位置。 此属性仅针对使用 `\security` 查询路径而不是查询路径 `\privacy` 访问的 API 定义。|
| pauseAfterEstimate   | 布尔值| 估计完成后暂停请求。 默认情况下，数据估算将运行，然后暂停，允许你预览结果，然后选择用于检索 UI 中数据的选项。 如果希望此属性 `false` 执行估算，则可以将其设置为自动开始检索内容。 此属性仅针对使用 `\security` 查询路径而不是查询路径 `\privacy` 访问的 API 定义。|
|法规|String collection|请求的一个或多个法规。|
| siteLocations| [subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md)| 应搜索的SharePoint和OneDrive站点位置。 此属性仅针对使用 `\security` 查询路径而不是查询路径 `\privacy` 访问的 API 定义。|
|type|subjectRightsRequestType|请求的类型。 可取值为：`export`、`access`、`tagForAction`、`unknownFutureValue`。 当前不支持该 `delete` 类型。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subjectRightsRequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/privacy/subjectRightsRequests
Content-Type: application/json

{
    "type": "export",
    "contentQuery": "((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))",
    "dataSubjectType": "customer",
    "externalId": "F53BF2DA-607D-412A-B568-FAA0F023AC0B",
    "displayName": "Export report for customer Id: 12345",
    "description": "This is a export request",
    "includeAllVersions": false,
    "includeAuthoredContent": true,
    "internalDueDateTime": "2022-07-20T22:42:28Z",
    "dataSubject": {
        "firstName": "Diego",
        "lastName": "Siciliani",
        "email": "Diego.Siciliani@contoso.com",
        "residency": "USA"
    },
    "mailboxLocations": null,
    "pauseAfterEstimate": true,
    "regulations": [
        "CCPA"
    ],
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestAllSiteLocation"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subjectrightsrequest-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subjectrightsrequest-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subjectrightsrequest-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-subjectrightsrequest-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subjectRightsRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "type": "export",
    "dataSubjectType": "customer",
    "regulations": [
        "CCPA"
    ],
    "displayName": "Export report for customer Id: 12345",
    "description": "This is a export request",
    "status": "active",
    "internalDueDateTime": "2022-07-20T22:42:28Z",
    "lastModifiedDateTime": "2022-05-10T22:42:28Z",
    "id": "CA084038-C5D2-493D-8DAB-23FC12393C76",
    "createdDateTime": "2022-05-10T22:42:28Z",
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "contentReview",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": null
        }
    ],
    "createdBy": {
        "user": {
            "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
            "displayName": "srradmin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
            "displayName": "srradmin@contoso.com"
        }
    },
    "dataSubject": {
        "firstName": "Diego",
        "lastName": "Siciliani",
        "email": "Diego.Siciliani@contoso.com",
        "residency": "USA"
    },
    "team": {
        "id": "5484809c-fb5b-415a-afc6-da7ff601034e",
        "webUrl": "https://teams.contoso.com/teams/teamid"
    },
    "includeAllVersions": false,
    "pauseAfterEstimate": false,
    "includeAuthoredContent": false,
    "externalId": "F53BF2DA-607D-412A-B568-FAA0F023AC0B",
    "contentQuery": "((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))",
    "mailboxLocations": null,
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestAllSiteLocation"
    }
}
```

