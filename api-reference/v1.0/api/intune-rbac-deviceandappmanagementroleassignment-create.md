---
title: 创建 deviceAndAppManagementRoleAssignment
description: 创建新的 deviceAndAppManagementRoleAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 261578bf213d2721d004b1db788bc510c53dd3ca
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455940"
---
# <a name="create-deviceandappmanagementroleassignment"></a>创建 deviceAndAppManagementRoleAssignment

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementRBAC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceAndAppManagementRoleAssignment 对象的 JSON 表示形式。

下表显示创建 deviceAndAppManagementRoleAssignment 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 此为只读，且自动生成。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|displayName|String|角色分配的显示或友好名称。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|说明|String|角色分配的说明。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|resourceScopes|String collection|角色作用域成员安全组的 ID 列表。  这些是 Azure Active Directory 中的 ID。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|members|String collection|角色成员安全组的 ID 列表。 这些是 Azure Active Directory 中的 ID。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



