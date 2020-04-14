---
title: deviceManagementSettingIntegerConstraint 资源类型
description: 强制整数设置允许的值范围的约束
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5cd1778ca89ad02fa564ed6e57c3e14744635f0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453363"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a>deviceManagementSettingIntegerConstraint 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

强制整数设置允许的值范围的约束


继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|minimumValue|Int32|允许的最小值|
|maximumValue|Int32|允许的最大值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```



