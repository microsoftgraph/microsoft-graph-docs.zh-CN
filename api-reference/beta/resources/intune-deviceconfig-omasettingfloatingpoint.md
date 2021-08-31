---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d17ed3461a3d61f5daec52f0c4a1116c9b93f89f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803284"
---
# <a name="omasettingfloatingpoint-resource-type"></a>omaSettingFloatingPoint 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OMA 设置浮点定义。


继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|说明。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|secretReferenceValueId|String|用于查找解密密码的 ReferenceId。 此属性是只读的。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|isEncrypted|Boolean|指示值字段是否加密。 此属性是只读的。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|value|单个|值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": 4.2
}
```



