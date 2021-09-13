---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e32862181c9e6a92ee7f5ef88bd90c96d286fbb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148100"
---
# <a name="omasettingstringxml-resource-type"></a>omaSettingStringXml 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OMA 设置字符串 XML 定义。


继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|说明|String|说明。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|String|与 Value 属性关联的文件名 (*.xml)。|
|value|Binary|值。 （UTF8 编码的字节数组）|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```




