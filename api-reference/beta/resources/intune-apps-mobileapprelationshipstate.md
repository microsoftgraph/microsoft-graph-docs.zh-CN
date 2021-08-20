---
title: mobileAppRelationshipState 资源类型
description: 描述 UPN 和设备 ID 上下文中子应用的安装状态详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b3f5930a33b464b33e2d81af78b13a216e03311b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266945"
---
# <a name="mobileapprelationshipstate-resource-type"></a>mobileAppRelationshipState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述 UPN 和设备 ID 上下文中子应用的安装状态详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|sourceIds|String collection|源移动应用 ID 的集合。|
|targetId|字符串|相关目标应用的 ID。|
|targetDisplayName|字符串|相关目标应用的显示名称。|
|deviceId|String|相应的设备 ID。|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|目标应用的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|应用的安装状态详细信息。 可能的值是 `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` ：、、、、、、、、、、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` 、|
|errorCode|Int32|目标应用安装或卸载失败的错误代码。|
|targetLastSyncDateTime|DateTimeOffset|目标应用的上次同步时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppRelationshipState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationshipState",
  "sourceIds": [
    "String"
  ],
  "targetId": "String",
  "targetDisplayName": "String",
  "deviceId": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "targetLastSyncDateTime": "String (timestamp)"
}
```




