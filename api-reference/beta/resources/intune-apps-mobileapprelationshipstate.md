---
title: mobileAppRelationshipState 资源类型
description: 介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a0fb017ceb5401058ce776d8f020e0337a361f5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331789"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="e7ed4-103">mobileAppRelationshipState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7ed4-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="e7ed4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ed4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ed4-106">介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="e7ed4-107">属性</span><span class="sxs-lookup"><span data-stu-id="e7ed4-107">Properties</span></span>
|<span data-ttu-id="e7ed4-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7ed4-108">Property</span></span>|<span data-ttu-id="e7ed4-109">类型</span><span class="sxs-lookup"><span data-stu-id="e7ed4-109">Type</span></span>|<span data-ttu-id="e7ed4-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7ed4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ed4-111">sourceIds</span><span class="sxs-lookup"><span data-stu-id="e7ed4-111">sourceIds</span></span>|<span data-ttu-id="e7ed4-112">String collection</span><span class="sxs-lookup"><span data-stu-id="e7ed4-112">String collection</span></span>|<span data-ttu-id="e7ed4-113">源移动应用程序 id 的集合。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="e7ed4-114">targetId</span><span class="sxs-lookup"><span data-stu-id="e7ed4-114">targetId</span></span>|<span data-ttu-id="e7ed4-115">String</span><span class="sxs-lookup"><span data-stu-id="e7ed4-115">String</span></span>|<span data-ttu-id="e7ed4-116">相关目标应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-116">The related target app's id.</span></span>|
|<span data-ttu-id="e7ed4-117">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="e7ed4-117">targetDisplayName</span></span>|<span data-ttu-id="e7ed4-118">String</span><span class="sxs-lookup"><span data-stu-id="e7ed4-118">String</span></span>|<span data-ttu-id="e7ed4-119">相关目标应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-119">The related target app's display name.</span></span>|
|<span data-ttu-id="e7ed4-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="e7ed4-120">deviceId</span></span>|<span data-ttu-id="e7ed4-121">String</span><span class="sxs-lookup"><span data-stu-id="e7ed4-121">String</span></span>|<span data-ttu-id="e7ed4-122">相应的设备 id。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-122">The corresponding device id.</span></span>|
|<span data-ttu-id="e7ed4-123">installState</span><span class="sxs-lookup"><span data-stu-id="e7ed4-123">installState</span></span>|[<span data-ttu-id="e7ed4-124">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e7ed4-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e7ed4-125">目标应用的应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-125">The install state of the app of target app.</span></span> <span data-ttu-id="e7ed4-126">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e7ed4-127">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="e7ed4-127">installStateDetail</span></span>|[<span data-ttu-id="e7ed4-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="e7ed4-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="e7ed4-129">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-129">The install state detail of the app.</span></span> <span data-ttu-id="e7ed4-130">可能的值为`noAdditionalDetails`: `dependencyFailedToInstall`、 `dependencyWithRequirementsNotMet`、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`、、、、、、、、、、、、、、、、 `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e7ed4-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="e7ed4-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="e7ed4-131">errorCode</span></span>|<span data-ttu-id="e7ed4-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ed4-132">Int32</span></span>|<span data-ttu-id="e7ed4-133">目标应用安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="e7ed4-134">targetLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ed4-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="e7ed4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ed4-135">DateTimeOffset</span></span>|<span data-ttu-id="e7ed4-136">目标应用程序的上次同步时间。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7ed4-137">关系</span><span class="sxs-lookup"><span data-stu-id="e7ed4-137">Relationships</span></span>
<span data-ttu-id="e7ed4-138">无</span><span class="sxs-lookup"><span data-stu-id="e7ed4-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7ed4-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7ed4-139">JSON Representation</span></span>
<span data-ttu-id="e7ed4-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7ed4-140">Here is a JSON representation of the resource.</span></span>
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



