---
title: windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 资源类型
description: 包含设备 WindowsDefenderApplicationControl 补充策略的部署状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01acfd4848732213e6fc4121209684dc021f1450a5223e6b7f17d9f9b62b1483
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54181067"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-resource-type"></a>windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备 WindowsDefenderApplicationControl 补充策略的部署状态的属性。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-list.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 集合|列出 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象的属性和关系。|
|[获取 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|读取 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象的属性和关系。|
|[创建 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-create.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|创建新的 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象。|
|[删除 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-delete.md)|无|删除 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)。|
|[更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|更新 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 对象](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceName|String|设备名称。|
|deviceId|String|设备 ID。|
|lastSyncDateTime|DateTimeOffset|上次同步日期时间。|
|osVersion|String|Windows操作系统版本。|
|osDescription|String|Windows操作系统版本说明。|
|deploymentStatus|[windowsDefenderApplicationControlSupplementalPolicyStatuses](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|策略的部署状态。 可取值为：`unknown`、`success`、`tokenError`、`notAuthorizedByToken`、`policyNotFound`。|
|userName|String|此设备的用户的名称。|
|userPrincipalName|字符串|用户主体名称。|
|policyVersion|字符串|WindowsDefenderApplicationControl 补充策略的可读版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|策略|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|指向 WindowsDefenderApplicationControl 补充策略的导航链接。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osVersion": "String",
  "osDescription": "String",
  "deploymentStatus": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "policyVersion": "String"
}
```




