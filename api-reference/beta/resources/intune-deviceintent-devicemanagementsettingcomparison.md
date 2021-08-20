---
title: deviceManagementSettingComparison 资源类型
description: 表示设置比较结果的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28ca971dbfa41c9237ed9f6ff33579d5e9f4eeb5f2b32dbf0ffd3b0eca191424
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156203"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>deviceManagementSettingComparison 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设置比较结果的实体

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设置 ID|
|displayName|字符串|设置显示名称|
|definitionId|字符串|此实例的设置定义的 ID|
|currentValueJson|String|当前意图的 JSON 表示 (或) 模板设置的值|
|newValueJson|String|新模板设置值的 JSON 表示形式|
|comparisonResult|[deviceManagementComparisonResult](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|设置比较结果。 可取值为：`unknown`、`equal`、`notEqual`、`added`、`removed`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```




