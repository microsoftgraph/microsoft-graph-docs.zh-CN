---
title: windowsManagementAppHealthSummary 资源类型
description: 包含 Windows management 应用的运行状况摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8033f5e66928de4e0f913eaaab0aaa271fa2894
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983979"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a>windowsManagementAppHealthSummary 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Windows management 应用的运行状况摘要的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|读取[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性和关系。|
|[更新 windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Windows management 应用运行状况摘要实体的键。|
|healthyDeviceCount|Int32|正常的设备计数。|
|unhealthyDeviceCount|Int32|设备计数不正常。|
|unknownDeviceCount|Int32|未知设备计数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```





