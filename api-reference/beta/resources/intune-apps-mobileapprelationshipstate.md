---
title: mobileAppRelationshipState 资源类型
description: 介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6013482fe69aa7a4ccf789c677ef448e0a277991
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993352"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="be50e-103">mobileAppRelationshipState 资源类型</span><span class="sxs-lookup"><span data-stu-id="be50e-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="be50e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be50e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be50e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be50e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be50e-106">介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="be50e-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="be50e-107">属性</span><span class="sxs-lookup"><span data-stu-id="be50e-107">Properties</span></span>
|<span data-ttu-id="be50e-108">属性</span><span class="sxs-lookup"><span data-stu-id="be50e-108">Property</span></span>|<span data-ttu-id="be50e-109">类型</span><span class="sxs-lookup"><span data-stu-id="be50e-109">Type</span></span>|<span data-ttu-id="be50e-110">说明</span><span class="sxs-lookup"><span data-stu-id="be50e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be50e-111">sourceIds</span><span class="sxs-lookup"><span data-stu-id="be50e-111">sourceIds</span></span>|<span data-ttu-id="be50e-112">String collection</span><span class="sxs-lookup"><span data-stu-id="be50e-112">String collection</span></span>|<span data-ttu-id="be50e-113">源移动应用程序 id 的集合。</span><span class="sxs-lookup"><span data-stu-id="be50e-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="be50e-114">targetId</span><span class="sxs-lookup"><span data-stu-id="be50e-114">targetId</span></span>|<span data-ttu-id="be50e-115">String</span><span class="sxs-lookup"><span data-stu-id="be50e-115">String</span></span>|<span data-ttu-id="be50e-116">相关目标应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="be50e-116">The related target app's id.</span></span>|
|<span data-ttu-id="be50e-117">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="be50e-117">targetDisplayName</span></span>|<span data-ttu-id="be50e-118">String</span><span class="sxs-lookup"><span data-stu-id="be50e-118">String</span></span>|<span data-ttu-id="be50e-119">相关目标应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be50e-119">The related target app's display name.</span></span>|
|<span data-ttu-id="be50e-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="be50e-120">deviceId</span></span>|<span data-ttu-id="be50e-121">String</span><span class="sxs-lookup"><span data-stu-id="be50e-121">String</span></span>|<span data-ttu-id="be50e-122">相应的设备 id。</span><span class="sxs-lookup"><span data-stu-id="be50e-122">The corresponding device id.</span></span>|
|<span data-ttu-id="be50e-123">installState</span><span class="sxs-lookup"><span data-stu-id="be50e-123">installState</span></span>|[<span data-ttu-id="be50e-124">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="be50e-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="be50e-125">目标应用的应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="be50e-125">The install state of the app of target app.</span></span> <span data-ttu-id="be50e-126">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="be50e-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="be50e-127">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="be50e-127">installStateDetail</span></span>|[<span data-ttu-id="be50e-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="be50e-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="be50e-129">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="be50e-129">The install state detail of the app.</span></span> <span data-ttu-id="be50e-130">可能的值为`noAdditionalDetails`: `dependencyFailedToInstall`、 `dependencyWithRequirementsNotMet`、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`、、、、、、、、、、、、、、、、 `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="be50e-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="be50e-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="be50e-131">errorCode</span></span>|<span data-ttu-id="be50e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="be50e-132">Int32</span></span>|<span data-ttu-id="be50e-133">目标应用安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="be50e-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="be50e-134">targetLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="be50e-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="be50e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be50e-135">DateTimeOffset</span></span>|<span data-ttu-id="be50e-136">目标应用程序的上次同步时间。</span><span class="sxs-lookup"><span data-stu-id="be50e-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be50e-137">关系</span><span class="sxs-lookup"><span data-stu-id="be50e-137">Relationships</span></span>
<span data-ttu-id="be50e-138">无</span><span class="sxs-lookup"><span data-stu-id="be50e-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be50e-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be50e-139">JSON Representation</span></span>
<span data-ttu-id="be50e-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be50e-140">Here is a JSON representation of the resource.</span></span>
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





