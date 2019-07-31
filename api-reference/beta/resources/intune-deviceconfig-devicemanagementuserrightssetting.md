---
title: deviceManagementUserRightsSetting 资源类型
description: 代表用户权限设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e041966f141ada4ca584d1c90cf9e1bd1af1f108
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001570"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a>deviceManagementUserRightsSetting 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表用户权限设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|表示此用户权限设置的当前状态。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|localUsersOrGroups|[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合|表示将在设备上设置的本地用户或组的集合 (如果允许此设置的状态)。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```





