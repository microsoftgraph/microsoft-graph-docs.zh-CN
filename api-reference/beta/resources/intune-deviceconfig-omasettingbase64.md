---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8b99c13b898bc2832d8e9f459b0adc95d55a772
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086636"
---
# <a name="omasettingbase64-resource-type"></a>omaSettingBase64 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OMA 设置 Base64 定义。


继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|说明|String|说明。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|secretReferenceValueId|String|用于查找解密密码的 ReferenceId。 此属性是只读的。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|isEncrypted|Boolean|指示值字段是否加密。 此属性是只读的。 继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|String|与 Value 属性 (*.cer | *.crt | *.p7b | *.bin) 。|
|value|String|值。 （Base64 编码字符串）|

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
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```



