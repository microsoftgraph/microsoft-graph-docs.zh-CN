---
title: 列出 ediscoveryFiles
description: 获取 ediscoveryFile 对象及其属性的列表。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 9e529a8f3366246f228eca43e9afdd4e64d19973
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093600"
---
# <a name="list-ediscoveryfiles"></a>列出 ediscoveryFiles
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [ediscoveryFile](../resources/security-ediscoveryfile.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ediscoveryFile](../resources/security-ediscoveryfile.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files?$top=5
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoveryfile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoveryfile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-ediscoveryfile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-ediscoveryfile-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryFile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/reviewSets('273f11a1-17aa-419c-981d-ff10d33e420f')/files",
    "@odata.nextLink": "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files?$top=5&$skiptoken=1",
    "value": [
        {
            "id": "000168cdf05c48d98faac7bff8719726a25da40bb2b9c369fb580b8797abf661",
            "dateTime": "2017-11-02T15:07:10Z",
            "size": 921,
            "name": "Report/CustomVisuals/WordCloud1447959067750/package.json",
            "sourceType": "site",
            "subjectTitle": "Operations Analytics.pbix",
            "extension": "json",
            "mediaType": "application/json; charset=ISO-8859-1",
            "processingStatus": "success",
            "otherProperties": {
                "Source": null,
                "Participants": null,
                "To": null,
                "Cc": null,
                "Bcc": null,
                "Recipients": null,
                "Author": null,
                "CreatedTime": null,
                "Received": null,
                "Sent": null,
                "LastModifiedDate": "2017-11-02T15:07:10Z",
                "MessageType": null,
                "Title": null,
                "EmailHasAttachment": false,
                "EmailImportance": "",
                "WordCount": 25,
                "ErrorIgnored": false,
                "IsFromErrorRemediation": false,
                "EmailSecurity": 0,
                "EmailSensitivity": 0,
                "IsModernAttachment": false,
                "IsEmbeddedDocument": true,
                "ComplianceLabels": null,
                "ConversationId": null,
                "ConversationIndex": null,
                "ItemClass": null,
                "LocationName": null,
                "MeetingStartDate": null,
                "MeetingEndDate": null,
                "ParticipantDomains": null,
                "RecipientDomains": null,
                "Sender": null,
                "SenderDomain": null
            }
        }
    ]
}
```

