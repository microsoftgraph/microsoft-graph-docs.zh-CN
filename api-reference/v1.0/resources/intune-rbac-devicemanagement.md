---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4b06bb4f6f9fdc55540c8a2361acf4afd6eeffa420b30e424b7d67417613e53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235462"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备管理功能的容器的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-rbac-devicemanagement-get.md)|[deviceManagement](../resources/intune-rbac-devicemanagement.md)|读取 [deviceManagement](../resources/intune-rbac-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-rbac-devicemanagement-update.md)|[deviceManagement](../resources/intune-rbac-devicemanagement.md)|更新 [deviceManagement](../resources/intune-rbac-devicemanagement.md) 对象的属性。|
|[getEffectivePermissions 函数](../api/intune-rbac-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md) 集合|检索当前验证的用户的有效权限|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合|角色定义。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合|角色分配。|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合|资源操作。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




