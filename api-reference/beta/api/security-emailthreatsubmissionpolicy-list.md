---
title: 列出 emailThreatSubmissionPolicies
description: 获取 emailThreatSubmissionPolicy 对象及其属性的列表。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 445660425e0c71fc0217006ab8d81e1f25cc9c34
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856525"
---
# <a name="list-emailthreatsubmissionpolicies"></a>列出 emailThreatSubmissionPolicies
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ThreatSubmission.Read、ThreatSubmission.ReadWrite、ThreatSubmission.Read.All、ThreatSubmission.ReadWrite.All、ThreatSubmissionPolicies.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|ThreatSubmission.Read.All、ThreatSubmission.ReadWrite.All、ThreatSubmissionPolicy.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET security/threatSubmission/emailThreatSubmissionPolicies
```

## <a name="optional-query-parameters"></a>可选的查询参数
不支持。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_emailthreatsubmissionpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.emailThreatSubmissionPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security.emailThreatSubmissionPolicy",
      "id": "3df67ecc-11b4-b5b4-9bae-b0729940b3d1",
      "isReportToMicrosoftEnabled": "Boolean",
      "isReportToCustomizedEmailAddressEnabled": "Boolean",
      "isAskMeEnabledForUsers": "Boolean",
      "isAlwaysReportEnabledForUsers": "Boolean",
      "isNeverReportEnabledForUsers": "Boolean",
      "isCustomizedMessageEnabledForPhishing": "Boolean",
      "isCustomizedMessageEnabled": "Boolean",
      "customizedReportRecipientEmailAddress": "String",
      "isReviewEmailNotificationEnabled": "Boolean",
      "isCustomizedNotificationSenderEnabled": "Boolean",
      "isOrganizationBrandingEnabled": "Boolean",
      "customizedNotificationSenderEmailAddress": "String",
      "isReportFromQuarantineEnabled": "Boolean"
    }
  ]
}
```

