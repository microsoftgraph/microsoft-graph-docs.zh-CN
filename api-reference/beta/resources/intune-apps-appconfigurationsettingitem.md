---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c08967a538577ccbaac68ab3964dea61dc18ac79
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798159"
---
# <a name="appconfigurationsettingitem-resource-type"></a>appConfigurationSettingItem 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含应用配置设置项的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appConfigKey|String|应用配置密钥。|
|appConfigKeyType|[mdmAppConfigKeyType](../resources/intune-apps-mdmappconfigkeytype.md)|应用配置密钥类型。 可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。|
|appConfigKeyValue|String|应用配置密钥值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



