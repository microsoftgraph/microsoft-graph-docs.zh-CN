---
title: deviceManagementConfigurationStringSettingValueDefinition 资源类型
description: 字符串约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7602bccd66669f9b54c8bad06bb17ac350f641b4
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671503"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>deviceManagementConfigurationStringSettingValueDefinition 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

字符串约束


继承自 [deviceManagementConfigurationSettingValueDefinition](../resources/intune-shared-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|format|[deviceManagementConfigurationStringFormat](../resources/intune-shared-devicemanagementconfigurationstringformat.md)|字符串的预定义格式。 可能的值为：、、、`ip``guid`、`base64`、`url`、`version`、`xml`、`time``date`、`binary``regEx`、、`json``dateTime`、。 `surfaceHub``email``none`|
|inputValidationSchema|String|正则表达式或输入字符串应匹配的任何 xml 或 json 架构|
|maximumLength|Int64|字符串的最大长度|
|minimumLength|Int64|字符串的最小长度|
|isSecret|Boolean|指定是否需要将设置视为机密。 标记为“是”的设置将在传输和静态中加密，并在 UX 中表示时显示为星号。|

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




