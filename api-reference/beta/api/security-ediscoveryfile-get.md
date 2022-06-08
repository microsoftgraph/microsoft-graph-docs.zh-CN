---
title: 获取 ediscoveryFile
description: 读取 ediscoveryFile 对象的属性和关系。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 665a28c1513a8d7d8feb7ac23af9893626f5963c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945142"
---
# <a name="get-ediscoveryfile"></a>获取 ediscoveryFile
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [ediscoveryFile](../resources/security-ediscoveryfile.md) 对象的属性和关系。

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files/{ediscoveryFileId}
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ediscoveryFile](../resources/security-ediscoveryfile.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "get_ediscoveryfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files/000168cdf05c48d98faac7bff8719726a25da40bb2b9c369fb580b8797abf661
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryFile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/reviewSets('273f11a1-17aa-419c-981d-ff10d33e420f')/files/$entity",
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
```

