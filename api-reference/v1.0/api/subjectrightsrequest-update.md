---
title: 更新 subjectRightsRequest
description: 更新 subjectRightsRequest 对象的属性。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9a67b3a6c8b2831bceda36207b99ce730f2383a2
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447958"
---
# <a name="update-subjectrightsrequest"></a>更新 subjectRightsRequest
命名空间：microsoft.graph

更新 [subjectRightsRequest 对象](../resources/subjectRightsRequest.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|SubjectRightsRequest.ReadWrite.All*|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持|

>[!IMPORTANT]
>标有星号* (*) 当前不可用。 有关详细信息，请参阅[已知问题](/graph/known-issues#compliance)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /privacy/subjectRightsRequests/{subjectRightsRequestId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象的 JSON 表示形式。

下表显示更新 [subjectRightsRequest 时所需的属性](../resources/subjectRightsRequest.md)。

|属性|类型|说明|
|:---|:---|:---|
|assignedTo|[microsoft.graph.identity](../resources/identity.md)|请求分配给的用户的标识信息。|
|说明|String|更新了请求的说明。|
|displayName|String|请求的更新名称。|
|internalDueDateTime|DateTimeOffset|更新了请求的内部截止日期。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_subjectRightsRequest"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/privacy/subjectRightsRequests/{subjectRightsRequestId}
Content-Type: application/json
Content-length: 837

{
  "@odata.type": "#microsoft.graph.subjectRightsRequest",
  "internalDueDateTime": "2021-08-30T00:00:00Z"
}
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subjectRightsRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "type": "microsoft.graph.subjectRightsRequestType",
    "dataSubjectType": "microsoft.graph.dataSubjectType",
    "regulations": [
        "String"
    ],
    "displayName": "String",
    "description": "String",
    "status": "active",
    "internalDueDateTime": "String",
    "lastModifiedDateTime": "String",
    "id": "String",
    "createdDateTime": "String",
    "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "dataSubject": {
        "firstName": "String",
        "lastName": "String",
        "email": "String",
        "residency": "String",
        "phoneNumber": "String",
        "SSN": "String"
    },
    "team": {
        "id": "String (identifier)",
        "webUrl": "String"
    }
}
```

