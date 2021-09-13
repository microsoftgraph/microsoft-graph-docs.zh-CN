---
title: deviceManagementConfigurationIntegerSettingValueDefinitionTemplate 资源类型
description: 整数设置值定义模板
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a39f6c3224487c826cbfd8dcabf6e4cb629b665
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069031"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinitiontemplate-resource-type"></a>deviceManagementConfigurationIntegerSettingValueDefinitionTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

整数设置值定义模板

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|minValue|Int32|整数设置最小值。 有效值 -2147483648 2147483647|
|maxValue|Int32|整数设置最大值。 有效值 -2147483648 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
  "minValue": 1024,
  "maxValue": 1024
}
```



