---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 分配给用户的角色定义和角色分配的集合。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: beadac8ef20d1a716369626c52664af3ef8d9042
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967670"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>deviceAndAppManagementAssignedRoleDetails 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

分配给用户的角色定义和角色分配的集合。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|roleDefinitionIds|String collection|分配给用户的表列角色定义的角色定义 Id。|
|roleAssignmentIds|String collection|分配给用户的表列角色分配的角色分配 Id。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```





