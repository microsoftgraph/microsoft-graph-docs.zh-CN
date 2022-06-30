---
title: 列出 retentionLabels
description: 获取 retentionLabel 对象及其属性的列表。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0981779968e9e4a7336333c48cddb2921431d5de
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439675"
---
# <a name="list-retentionlabels"></a>列出 retentionLabels
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [retentionLabel](../resources/security-retentionlabel.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RecordsManagement.Read.All、RecordsManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|RecordsManagement.Read.All、RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/labels/retentionLabels
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持展开 OData 查询参数，以帮助自定义响应。  例如，若要检索 **retentionEventType** 属性，可以使用 `expand` 参数：`$expand=retentionEventType`。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_retentionlabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/labels/retentionLabels
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.retentionLabel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security.retentionLabel",
      "id": "64a99fb4-07be-0481-8746-44c15c0eef1f",
      "displayName": "String",
      "behaviorDuringRetentionPeriod": "String",
      "actionAfterRetentionPeriod": "String",
      "retentionTrigger": "String",
      "retentionDuration": {
        "@odata.type": "microsoft.graph.security.retentionDuration"
      },
      "isInUse": "Boolean",
      "descriptionForAdmins": "String",
      "descriptionForUsers": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "labelToBeApplied": "String",
      "defaultRecordBehavior": "String"
    }
  ]
}
```


