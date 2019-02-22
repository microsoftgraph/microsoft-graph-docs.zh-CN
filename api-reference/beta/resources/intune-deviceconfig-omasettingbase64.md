---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f6eae88e7158d5fd8d09caadda9fee6778182a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166645"
---
# <a name="omasettingbase64-resource-type"></a>omaSettingBase64 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OMA 设置 Base64 定义。


继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|显示名称。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|字符串|说明。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|字符串|OMA。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|String|与 Value 属性 (*.cer | * .crt | *. p7b | * bin)。|
|值|String|值。 （Base64 编码字符串）|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```




