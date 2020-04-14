---
title: deviceManagementSettingRegexConstraint 资源类型
description: 根据给定的 RegEx 模式强制设置匹配的约束
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82eb19727c839bf6c31f79d42fc9fbcf48b37f1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420098"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a>deviceManagementSettingRegexConstraint 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

根据给定的 RegEx 模式强制设置匹配的约束


继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|正则表达式|String|要匹配的正则表达式模式|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```



