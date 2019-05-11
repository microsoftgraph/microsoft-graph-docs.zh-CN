---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adfc465e607567c02f80b63760fa45e62466398b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950478"
---
# <a name="appconfigurationsettingitem-resource-type"></a>appConfigurationSettingItem 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




