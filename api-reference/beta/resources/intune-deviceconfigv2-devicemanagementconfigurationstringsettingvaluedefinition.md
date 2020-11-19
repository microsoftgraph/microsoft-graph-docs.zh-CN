---
title: deviceManagementConfigurationStringSettingValueDefinition 资源类型
description: 字符串约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03a96252cffabddd2acb613ff365fd16951fd55c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241538"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>deviceManagementConfigurationStringSettingValueDefinition 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

字符串约束


继承自 [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|format|[deviceManagementConfigurationStringFormat](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|预定义的字符串格式。 可能的值为：、、、、、、、、、、、、、、 `none` `email` `guid` `ip` `base64` `url` `version` `xml` `date` `time` `binary` `regEx` `json` `dateTime` `surfaceHub` 。|
|inputValidationSchema|String|输入字符串应匹配的正则表达式或任何 xml 或 json 架构|
|maximumLength|Int64|字符串的最大长度。 有效值为0至87516|
|Minimumheight|Int64|字符串的最小长度。 有效值为0至87516|
|isSecret|Boolean|指定是否需要将设置视为机密。 标记为 "是" 的设置将在传输过程中和 rest 中进行加密，并在 UX 中表示为星号时将显示为星号。|

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




