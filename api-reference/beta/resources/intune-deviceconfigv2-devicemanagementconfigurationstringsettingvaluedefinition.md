---
title: deviceManagementConfigurationStringSettingValueDefinition 资源类型
description: 字符串约束
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a497972c8d84781cb5984993389fdb1163514f0d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128842"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>deviceManagementConfigurationStringSettingValueDefinition 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

字符串约束


继承自 [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|format|[deviceManagementConfigurationStringFormat](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|预定义的字符串格式。 可能的值是 `none` `email` `guid` ：、、、、、、、、、、 `ip` `base64` `url` `version` `xml` `date` `time` `binary` `regEx` `json` `dateTime` `surfaceHub` 。|
|inputValidationSchema|String|输入字符串应匹配的正则表达式或任何 xml 或 json 架构|
|maximumLength|Int64|字符串的最大长度。 有效值为 0 到 87516|
|minimumLength|Int64|字符串的最小长度。 有效值为 0 到 87516|
|isSecret|Boolean|指定是否需要将设置视为机密。 设置标记为"是"的内容将在传输中和处于其余状态进行加密，并且将在 UX 中表示时显示为星号。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition",
  "format": "String",
  "inputValidationSchema": "String",
  "maximumLength": 1024,
  "minimumLength": 1024,
  "isSecret": true
}
```



