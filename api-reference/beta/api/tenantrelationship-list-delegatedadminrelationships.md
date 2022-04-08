---
title: 列出 delegatedAdminRelationships
description: 获取 delegatedAdminRelationship 对象及其属性的列表。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 4c8f47cf8d0204b51a26d318a951cf00f05c8b09
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704450"
---
# <a name="list-delegatedadminrelationships"></a>列出 delegatedAdminRelationships
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.Read.All、DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminRelationships
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select`[OData](/graph/query-parameters) `$filter``$orderBy``$top`查询参数，`$count``$skipToken`以帮助自定义响应。  

`$top` 最多支持 300 个对象。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 对象的集合。

每个 **delegatedAdminRelationship** 对象都包含 **一个 @odata.etag** 属性（根据 RFC2616）。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_delegatedadminrelationship"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminRelationship)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminRelationships",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMDAwLTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836",
      "displayName": "Contoso admin relationship",
      "duration": "P730D",
      "customer": {
        "tenantId": "52eaad04-13a2-4a2f-9ce8-93a294fadf36",
        "displayName": "Contoso Inc"
      },
      "accessDetails": {
        "unifiedRoles": [
          {
            "roleDefinitionId": "dd4db9a0-cc4a-4213-9f9f-70242232d97e"
          }
        ]
      },
      "status": "active",
      "createdDateTime": "2022-02-10T11:24:42.3148266Z",
      "lastModifiedDateTime": "2022-02-10T11:26:44.9941884Z",
      "activatedDateTime": "2022-02-10T11:26:44.9941884Z",
      "endDateTime": "2024-02-10T11:24:42.3148266Z"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wKklILTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "1041ef52-a99b-4245-a3be-cbd3fa7c5ed1-8777b240-c6f0-4469-9e98-a3205431b836",
      "displayName": "Contoso subsidiary relationship",
      "duration": "P30D",
      "customer": {
        "tenantId": "4b827261-d21f-4aa9-b7db-7fa1f56fb163",
        "displayName": "Contoso subsidiary Inc"
      },
      "accessDetails": {
        "unifiedRoles": [
          {
            "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
          },
          {
            "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
          }
        ]
      },
      "status": "terminated",
      "createdDateTime": "2021-09-29T16:52:39.6133896Z",
      "lastModifiedDateTime": "2021-10-29T16:57:20.2101088Z",
      "activatedDateTime": "2021-09-29T16:55:20.2101088Z",
      "endDateTime": "2021-10-29T16:57:20.2101088Z"
    }
  ]
}
```

