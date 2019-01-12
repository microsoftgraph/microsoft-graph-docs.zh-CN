---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组工作分配目标。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9d59a6adc5478d619187e5414ac92170cbdedd49
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926377"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>officeConfigurationGroupAssignmentTarget 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Office 客户端配置 AAD 组工作分配目标。

继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|groupId|字符串|AAD 组 Id 目标到该设备的配置。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



