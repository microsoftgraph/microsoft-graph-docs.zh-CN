---
title: androidFotaDeploymentAssignment 资源类型
description: 介绍要向其分配部署的部署安全组。 在向 Zebra 发送创建部署请求之前，后端将展开安全组 ID 以提取设备序列号。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c159840ba5bb2035223a45f0dec54a94055a2176
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213175"
---
# <a name="androidfotadeploymentassignment-resource-type"></a>androidFotaDeploymentAssignment 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍要向其分配部署的部署安全组。 在向 Zebra 发送创建部署请求之前，后端将展开安全组 ID 以提取设备序列号。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| Android FOTA 分配实体的密钥|
|target|[androidFotaDeploymentAssignmentTarget](../resources/intune-androidfotaservice-androidfotadeploymentassignmenttarget.md)|要将固件更新部署到的AAD组|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidFotaDeploymentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
    "groupId": "String"
  }
}
```




