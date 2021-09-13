---
title: deviceManagementConfigurationReferenceSettingValue 资源类型
description: ReferenceSettingValue 的模型
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12b6e60b63be0303603c63fa359bbdcc1820606d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148219"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a>deviceManagementConfigurationReferenceSettingValue 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ReferenceSettingValue 的模型


继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|设置值模板引用 继承自 [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|
|value|String|字符串设置的值。 继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)|
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
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String",
  "note": "String"
}
```



