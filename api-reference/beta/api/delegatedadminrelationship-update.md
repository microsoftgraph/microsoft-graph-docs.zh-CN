---
title: 更新 delegatedAdminRelationship
description: 更新 delegatedAdminRelationship 对象的属性。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 3287d707ad45c8adf693b354bfeb8e34be52e12c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203158"
---
# <a name="update-delegatedadminrelationship"></a>更新 delegatedAdminRelationship
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [delegatedAdminRelationship 对象的](../resources/delegatedadminrelationship.md) 属性。 仅当关系处于 **状态** 时`created`，才能更新关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|Application| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|If-Match|If-match： {etag}。 要更新的 **delegatedAdminRelationship** 的最后一个已知 ETag 值。 从 LIST 或 GET 操作中检索 ETag 值。 必填。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|accessDetails|[microsoft.graph.delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|合作伙伴在客户租户中请求或有权访问的管理角色的标识符。|
|客户|[microsoft.graph.delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|关系客户的显示名称和唯一标识符。|
|displayName|String|用于简化标识的关系的显示名称。 在合作伙伴 *的所有* 委派管理员关系中必须是唯一的。|
|duration|期限|以 ISO 8601 格式的关系持续时间。 必须是介于和`P2Y`非独占之间的`P1D`值。|


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新 [的 delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_delegatedadminrelationship"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836
If-Match: W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="
Content-Type: application/json

{
  "displayName": "Updated Contoso admin relationship",
  "duration": "P31D",
  "customer": {
    "tenantId": "52eaad04-13a2-4a2f-9ce8-93a294fadf36"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a"
      },
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "69091246-20e8-4a56-aa4d-066075b2a7a8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-delegatedadminrelationship-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-delegatedadminrelationship-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-delegatedadminrelationship-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-delegatedadminrelationship-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-delegatedadminrelationship-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationship"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminRelationships/$entity",
  "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMDAwLTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
  "id": "5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836",
  "displayName": "Updated Contoso admin relationship",
  "duration": "P31D",
  "status": "created",
  "createdDateTime": "2022-02-10T11:24:42.3148266Z",
  "lastModifiedDateTime": "2022-02-10T11:26:44.9941884Z",
  "customer": {
    "tenantId": "52eaad04-13a2-4a2f-9ce8-93a294fadf36"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a"
      },
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "69091246-20e8-4a56-aa4d-066075b2a7a8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```

