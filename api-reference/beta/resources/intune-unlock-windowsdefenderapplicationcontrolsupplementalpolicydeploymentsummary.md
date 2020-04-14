---
title: windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary 资源类型
description: 包含 WindowsDefenderApplicationControl 补充策略的部署摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c16cdd6518998f6979260462d844cefa072f2061
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449557"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-resource-type"></a>windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 WindowsDefenderApplicationControl 补充策略的部署摘要的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|读取[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)对象的属性和关系。|
|[更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|更新[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deployedDeviceCount|Int32|已成功部署此 WindowsDefenderApplicationControl 补充策略的设备数量。|
|failedDeviceCount|Int32|无法部署此 WindowsDefenderApplicationControl 补充策略的设备数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "id": "String (identifier)",
  "deployedDeviceCount": 1024,
  "failedDeviceCount": 1024
}
```



