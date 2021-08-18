---
title: deviceAndAppManagementAssignmentTarget 资源类型
description: 赋值目标的基类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4f2c48e000e698c7b97bea4456c84aa991ad1d01301ed10bec896b529ccabda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54158164"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a>deviceAndAppManagementAssignmentTarget 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

赋值目标的基类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceAndAppManagementAssignmentFilterId|String|目标分配的筛选器 ID。|
|deviceAndAppManagementAssignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|目标分配的筛选器类型，即排除或包含。 可取值为：`none`、`include`、`exclude`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```




