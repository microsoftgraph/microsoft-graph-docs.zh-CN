---
title: mobileAppRelationshipState 资源类型
description: 介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: daca7e69b70ccfecef181dd0bdd4eb381f010d87
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792700"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="1cd62-103">mobileAppRelationshipState 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cd62-103">mobileAppRelationshipState resource type</span></span>

<span data-ttu-id="1cd62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cd62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cd62-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1cd62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cd62-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cd62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd62-107">介绍 UPN 和设备 id 上下文中的子应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="1cd62-107">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="1cd62-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cd62-108">Properties</span></span>
|<span data-ttu-id="1cd62-109">属性</span><span class="sxs-lookup"><span data-stu-id="1cd62-109">Property</span></span>|<span data-ttu-id="1cd62-110">类型</span><span class="sxs-lookup"><span data-stu-id="1cd62-110">Type</span></span>|<span data-ttu-id="1cd62-111">说明</span><span class="sxs-lookup"><span data-stu-id="1cd62-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd62-112">sourceIds</span><span class="sxs-lookup"><span data-stu-id="1cd62-112">sourceIds</span></span>|<span data-ttu-id="1cd62-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1cd62-113">String collection</span></span>|<span data-ttu-id="1cd62-114">源移动应用程序 id 的集合。</span><span class="sxs-lookup"><span data-stu-id="1cd62-114">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="1cd62-115">targetId</span><span class="sxs-lookup"><span data-stu-id="1cd62-115">targetId</span></span>|<span data-ttu-id="1cd62-116">String</span><span class="sxs-lookup"><span data-stu-id="1cd62-116">String</span></span>|<span data-ttu-id="1cd62-117">相关目标应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="1cd62-117">The related target app's id.</span></span>|
|<span data-ttu-id="1cd62-118">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="1cd62-118">targetDisplayName</span></span>|<span data-ttu-id="1cd62-119">String</span><span class="sxs-lookup"><span data-stu-id="1cd62-119">String</span></span>|<span data-ttu-id="1cd62-120">相关目标应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1cd62-120">The related target app's display name.</span></span>|
|<span data-ttu-id="1cd62-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="1cd62-121">deviceId</span></span>|<span data-ttu-id="1cd62-122">String</span><span class="sxs-lookup"><span data-stu-id="1cd62-122">String</span></span>|<span data-ttu-id="1cd62-123">相应的设备 id。</span><span class="sxs-lookup"><span data-stu-id="1cd62-123">The corresponding device id.</span></span>|
|<span data-ttu-id="1cd62-124">installState</span><span class="sxs-lookup"><span data-stu-id="1cd62-124">installState</span></span>|[<span data-ttu-id="1cd62-125">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="1cd62-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="1cd62-126">目标应用的应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="1cd62-126">The install state of the app of target app.</span></span> <span data-ttu-id="1cd62-127">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="1cd62-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="1cd62-128">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="1cd62-128">installStateDetail</span></span>|[<span data-ttu-id="1cd62-129">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="1cd62-129">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="1cd62-130">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="1cd62-130">The install state detail of the app.</span></span> <span data-ttu-id="1cd62-131">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、 `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` 。</span><span class="sxs-lookup"><span data-stu-id="1cd62-131">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="1cd62-132">errorCode</span><span class="sxs-lookup"><span data-stu-id="1cd62-132">errorCode</span></span>|<span data-ttu-id="1cd62-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd62-133">Int32</span></span>|<span data-ttu-id="1cd62-134">目标应用安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="1cd62-134">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="1cd62-135">targetLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd62-135">targetLastSyncDateTime</span></span>|<span data-ttu-id="1cd62-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd62-136">DateTimeOffset</span></span>|<span data-ttu-id="1cd62-137">目标应用程序的上次同步时间。</span><span class="sxs-lookup"><span data-stu-id="1cd62-137">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cd62-138">关系</span><span class="sxs-lookup"><span data-stu-id="1cd62-138">Relationships</span></span>
<span data-ttu-id="1cd62-139">无</span><span class="sxs-lookup"><span data-stu-id="1cd62-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cd62-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cd62-140">JSON Representation</span></span>
<span data-ttu-id="1cd62-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cd62-141">Here is a JSON representation of the resource.</span></span>
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



