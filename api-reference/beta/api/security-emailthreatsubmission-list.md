---
title: 列出 emailThreatSubmissions
description: 获取 emailThreatSubmission 对象及其属性的列表。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f1fa1262f71974e77b03c795b52833c8b3455f42
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856522"
---
# <a name="list-emailthreatsubmissions"></a>列出 emailThreatSubmissions
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [emailThreatSubmission](../resources/security-emailthreatsubmission.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ThreatSubmission.Read、ThreatSubmission.ReadWrite、ThreatSubmission.Read.All、ThreatSubmission.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|ThreatSubmission.Read.All、ThreatSubmission.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/threatSubmission/emailThreats
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持`$filter``$top`并 `$skipToken` `$count`帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [emailThreatSubmission](../resources/security-emailthreatsubmission.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_emailthreatsubmission"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/threatSubmission/emailThreats
```


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.emailThreatSubmission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/threatSubmission/emailThreats",
    "value": [
        {
            "@odata.type": "#microsoft.graph.emailThreatSubmission",
            "category": "spam",
            "recipientEmailAddress": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
            "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
            "createdDateTime": "2021-10-10T03:30:18.6890937Z",
            "contentType": "email",
            "emailSubject": "This is a spam",
            "status": "succeeded",
            "source": "administrator",
            "createdBy": {
                "user": {
                    "identity": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
                    "displayName": "Ronald Admin",
                    "email": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com"
                }
            },
            "result": {
            "detail": "allowedByTenant",
            "category": "notSpam",
            "userMailboxSetting": "isFromDomainInDomainSafeList,isJunkMailRuleEnabled",
            "detectedUrls": ["contoso.com"],
            "detectedFiles": [
                {
                    "fileName": "test.ps1",
                    "fileHash": "hash of test.ps1"
                }
            ]
            },
            "adminReview": null,
            "internetMessageId": "some-internet-message-id@contoso.com",
            "sender": "test@contoso.com",
            "senderIP": "127.0.0.1",
            "receivedDateTime": "2021-10-09T03:30:18.6890937Z",
            "originalCategory": "notSpam",
            "attackSimulationInfo": null,
            "tenantAllowOrBlockListAction": 
            {
                "action": "allow",
                "expirationDateTime": "2021-10-30T03:30:18.6890937Z",
                "note": "temporal allow the url/attachment/sender in the email.",
                "results": [
                    {
                        "identity": "tenant allow block list id",
                        "value": "contoso.com",
                        "entryType": "url",
                        "expirationDateTime": "2021-10-30T03:30:18.6890937Z",
                        "status": "succeeded"
                    },
                    {
                        "identity": "tenant allow block list id",
                        "value": "test-contoso.com",
                        "entryType": "url",
                        "expirationDateTime": "2021-10-30T03:30:18.6890937Z",
                        "status": "skipped"
                    },
                ]
            },
            "tenantId" : "39238e87-b5ab-4ef6-a559-af54c6b07b42"
        }
    ]
}
```

