---
title: deviceManagementConfigurationReferredSettingInformation 资源类型
description: 有关可重用设置的参考设置信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12003df5ec19bdf32b213945033eb9d5e73b9692
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868391"
---
# <a name="devicemanagementconfigurationreferredsettinginformation-resource-type"></a>deviceManagementConfigurationReferredSettingInformation 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

有关可重用设置的参考设置信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settingDefinitionId|String|设置引用到设置的定义 ID。 适用于可重用设置|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
  "settingDefinitionId": "String"
}
```




