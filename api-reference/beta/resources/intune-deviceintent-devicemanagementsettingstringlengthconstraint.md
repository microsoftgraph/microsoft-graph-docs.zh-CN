---
title: deviceManagementSettingStringLengthConstraint 资源类型
description: 强制实施给定字符串长度范围的约束
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7cdcdeb138dce2c5b201527a079e3ee2de03737
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984462"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a>deviceManagementSettingStringLengthConstraint 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

强制实施给定字符串长度范围的约束


继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|Minimumheight|Int32|允许的最小字符串长度|
|maximumLength|Int32|允许的最大字符串长度|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```





