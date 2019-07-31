---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组分配目标。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb97541a86e820e02e56a20568d3869a047dc2c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011958"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>officeConfigurationGroupAssignmentTarget 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Office 客户端配置 AAD 组分配目标。

继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|groupId|String|要将设备配置定向到的 AAD 组的 Id。|

## <a name="relationships"></a>关系
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



