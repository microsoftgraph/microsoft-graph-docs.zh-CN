---
title: deviceManagementConfigurationSettingInstanceTemplate 资源类型
description: 设置实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c89efaac6ff65f82c09ed787a9ed879d50e429386e61092021a9aff817a7724a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244846"
---
# <a name="devicemanagementconfigurationsettinginstancetemplate-resource-type"></a>deviceManagementConfigurationSettingInstanceTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设置实例模板

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settingInstanceTemplateId|字符串|设置实例模板 ID|
|settingDefinitionId|String|设置定义 ID|
|isRequired|Boolean|指示策略是否必须指定此设置。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true
}
```




