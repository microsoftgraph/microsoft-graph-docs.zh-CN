---
title: deviceManagementSettingDependency 资源类型
description: 设置的相关性信息
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9014b3618562717c2cc9522c388034ad81213a4c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420120"
---
# <a name="devicemanagementsettingdependency-resource-type"></a>deviceManagementSettingDependency 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设置的相关性信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|definitionId|String|设置的设置定义 ID 依赖于|
|施加|[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合|依赖项设置值的约束集合|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ]
}
```



