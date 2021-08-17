---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9c5349ecbbd9b61c1a5dacd5ac7006fe29f41a529c72f0bb0bf5e47a9d269a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54142195"
---
# <a name="appconfigurationsettingitem-resource-type"></a>appConfigurationSettingItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




