---
title: deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate 资源类型
description: 整数设置值常量默认模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31c775d857fdce4d1e416d99a33e35deae6a4606
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819883"
---
# <a name="devicemanagementconfigurationintegersettingvalueconstantdefaulttemplate-resource-type"></a>deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

整数设置值常量默认模板


继承自 [deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|constantValue|Int32|默认常量值。 有效值 -2147483648 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
  "constantValue": 1024
}
```



