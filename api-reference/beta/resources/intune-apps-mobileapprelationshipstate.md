---
title: mobileAppRelationshipState 资源类型
description: 介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b76572f56e219a08a7dc7452e184e31be121ae4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491342"
---
# <a name="mobileapprelationshipstate-resource-type"></a>mobileAppRelationshipState 资源类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|sourceIds|String 集合|源移动应用程序 id 的集合。|
|targetId|String|相关目标应用程序的 id。|
|targetDisplayName|String|相关目标应用程序的显示名称。|
|deviceId|String|相应的设备 id。|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|目标应用的应用程序的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|应用程序的安装状态详细信息。 可取值为：`noAdditionalDetails`、`dependencyFailedToInstall`、`dependencyWithRequirementsNotMet`、`dependencyPendingReboot`、`dependencyWithAutoInstallDisabled`、`seeInstallErrorCode`、`autoInstallDisabled`、`seeUninstallErrorCode`、`pendingReboot`、`installingDependencies`、`contentDownloaded`、`powerShellScriptRequirementNotMet`、`registryRequirementNotMet`、`fileSystemRequirementNotMet`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。|
|errorCode|Int32|目标应用安装或卸载失败的错误代码。|
|targetLastSyncDateTime|DateTimeOffset|目标应用程序的上次同步时间。|

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



