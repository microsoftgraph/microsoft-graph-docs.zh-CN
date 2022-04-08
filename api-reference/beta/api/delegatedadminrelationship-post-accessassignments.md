---
title: 创建 accessAssignments
description: 创建新的 delegatedAdminAccessAssignment 对象。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: f3faa2293b47f7837f016537563dfb8b6be77455
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704357"
---
# <a name="create-accessassignments"></a>创建 accessAssignments
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/accessAssignments
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [delegatedAdminAccessAssignment 对象的](../resources/delegatedadminaccessassignment.md) JSON 表示形式。

创建 **delegatedAdminAccessAssignment** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|分配成员访问权限的访问容器。 例如，安全组。|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|合作伙伴在客户租户中分配的管理角色的标识符。|


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 对象。 响应中的 **Location** 标头指向创建 **的 delegatedAdminAccessAssignment** 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_delegatedadminaccessassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments
Content-Type: application/json

{
  "accessContainer": {
    "accessContainerId": "869713c9-0b28-4d08-8949-ae07ae1bf528",
    "accessContainerType": "securityGroup"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
      },
      {
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments/a9d6cf90-083a-47dc-ace2-1da98be3f344

{

  "@odata.type": "#microsoft.graph.delegatedAdminAccessAssignment",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#accessAssignments",
  "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
  "id": "a9d6cf90-083a-47dc-ace2-1da98be3f344",
  "status": "pending",
  "createdDateTime": "2022-02-13T10:33:52.3182097Z",
  "lastModifiedDateTime": "2022-02-13T10:33:52.3182097Z",
  "accessContainer": {
    "accessContainerId": "869713c9-0b28-4d08-8949-ae07ae1bf528",
    "accessContainerType": "securityGroup"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
      },
      {
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```

