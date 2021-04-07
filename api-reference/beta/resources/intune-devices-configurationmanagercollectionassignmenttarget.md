---
title: configurationManagerCollectionAssignmentTarget 资源类型
description: 表示对 Configuration Manager 集合的分配。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb43c23a0eafaefea0b9265102880de58008f153
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610871"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a>configurationManagerCollectionAssignmentTarget 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示对 Configuration Manager 集合的分配。


继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|deviceAndAppManagementAssignmentFilterId|String|目标分配的筛选器 ID。 继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|
|deviceAndAppManagementAssignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|目标分配的筛选器类型，即排除或包含。 继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)。 可取值为：`none`、`include`、`exclude`。|
|collectionId|String|作为工作分配目标的集合 ID。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerCollectionAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "collectionId": "String"
}
```




