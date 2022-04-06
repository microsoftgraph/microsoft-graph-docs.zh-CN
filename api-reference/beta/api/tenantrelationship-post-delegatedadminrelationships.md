---
title: 创建 delegatedAdminRelationship
description: 创建新的 delegatedAdminRelationship 对象。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 052790ed1b5356d86316364017dab395e2ecc661
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589771"
---
# <a name="create-delegatedadminrelationship"></a>创建 delegatedAdminRelationship
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 对象。

## <a name="permissions"></a>Permissions
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
POST /tenantRelationships/delegatedAdminRelationships
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 对象的 JSON 表示形式。

可以在创建 **delegatedAdminRelationship 时指定以下属性**。

|属性|类型|说明|
|:---|:---|:---|
|accessDetails|[microsoft.graph.delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|合作伙伴在客户租户中请求或有权访问的管理角色的标识符。 必需项。|
|customer|[microsoft.graph.delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|关系显示名称的客户的标识符和唯一标识符。 可选。|
|displayName|String|用于显示名称识别的关系的标识。 在 *合作伙伴的所有委派* 管理员关系中必须是唯一的。 必需项。|
|duration|期限|关系采用 ISO 8601 格式的持续时间。 必须是介于 和 （包含 `P1D` 两者） `P2Y` 之间的值。 必需。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应 [代码和 delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 对象。

该响应包含 **一个 Location** 标头，其中包含指向已创建的委派管理员关系的 URL。 每个 **delegatedAdminRelationship** 对象都包含一个 **@odata.etag** 属性（根据 RFC2616）。
## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_delegatedadminrelationship_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships
Content-Type: application/json

{
  "displayName": "Contoso admin relationship",
  "duration": "P730D",
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
  }
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationship"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminRelationships",
  "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
  "id": "5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836",
  "displayName": "Contoso admin relationship",
  "duration": "P730D",
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
  "status": "created",
  "createdDateTime": "2022-02-10T11:24:42.3148266Z",
  "lastModifiedDateTime": "2022-02-10T11:24:42.3148266Z",
  "activatedDateTime": "",
  "endDateTime": "2024-02-10T11:24:42.3148266Z"
}
```

