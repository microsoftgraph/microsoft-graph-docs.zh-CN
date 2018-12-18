---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: tfitzmac
ms.openlocfilehash: 5582ca84a9d6c918ce7b8dea5a21f616804da4ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323784"
---
# <a name="omasettingstringxml-resource-type"></a>omaSettingStringXml 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

OMA 设置字符串 XML 定义。

继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|说明。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
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





