---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 分配给用户的角色定义和角色分配集。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b82d762d5c20d64f917729a193f2914c87acf040
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030128"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>deviceAndAppManagementAssignedRoleDetails 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

分配给用户的角色定义和角色分配集。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|roleDefinitionIds|String collection|分配给用户的指定角色定义的角色定义 ID。 此属性是只读的。|
|roleAssignmentIds|String collection|分配给用户的指定角色分配的角色分配 ID。 此属性是只读的。|

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



