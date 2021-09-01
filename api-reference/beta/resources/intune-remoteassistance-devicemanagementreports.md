---
title: deviceManagementReports 资源类型
description: 用于报告 V2 的 DeviceManagementReports 类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a726d3fb1cd0222e3a9939467e0d94ebb27df9c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820315"
---
# <a name="devicemanagementreports-resource-type"></a>deviceManagementReports 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于报告 V2 的 DeviceManagementReports 类

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[获取 deviceManagementReports](../api/intune-remoteassistance-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-remoteassistance-devicemanagementreports.md)|读取 [deviceManagementReports 对象的属性和](../resources/intune-remoteassistance-devicemanagementreports.md) 关系。|
|[更新 deviceManagementReports](../api/intune-remoteassistance-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-remoteassistance-devicemanagementreports.md)|更新 [deviceManagementReports 对象](../resources/intune-remoteassistance-devicemanagementreports.md) 的属性。|
|[getRemoteAssistanceSessionsReport 操作](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancesessionsreport.md)|Stream|尚未记录|
|[getRemoteAssistanceMonitorActiveSessionsReport 操作](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitoractivesessionsreport.md)|Stream|尚未记录|
|[getRemoteAssistanceMonitorTotalSessionsReport 操作](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitortotalsessionsreport.md)|Stream|尚未记录|
|[getRemoteAssistanceMonitorAvgSessionTimeReport 操作](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitoravgsessiontimereport.md)|Stream|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```



