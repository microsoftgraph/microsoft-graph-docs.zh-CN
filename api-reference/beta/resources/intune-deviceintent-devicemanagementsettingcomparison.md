---
title: deviceManagementSettingComparison 资源类型
description: 表示设置比较结果的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e8c886e3464070d0dba8779741ed65681a764de
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364738"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>deviceManagementSettingComparison 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设置比较结果的实体

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设置 ID|
|displayName|String|设置的显示名称|
|definitionId|String|此实例的设置定义的 ID|
|currentValueJson|String|当前意图 (或) 模板设置值的 JSON 表示形式|
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



