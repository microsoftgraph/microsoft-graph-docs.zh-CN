---
title: deviceManagementConfigurationReferenceSettingValue 资源类型
description: ReferenceSettingValue 的模型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1dc92606270cf4c2febcee68905f0c8bd29ced13
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868425"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a>deviceManagementConfigurationReferenceSettingValue 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ReferenceSettingValue 的模型


继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|值|String|字符串设置的值。 继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)|
|note|String|管理员可用于放入一些上下文信息的注释|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "value": "String",
  "note": "String"
}
```




