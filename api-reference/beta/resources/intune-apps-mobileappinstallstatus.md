---
title: mobileAppInstallStatus 资源类型
description: 包含设备的移动应用程序安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92e833def6b1b3c27a416039a56e1d818baad72f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071127"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="74598-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="74598-103">mobileAppInstallStatus resource type</span></span>

<span data-ttu-id="74598-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74598-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74598-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74598-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74598-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74598-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74598-107">包含设备的移动应用程序安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="74598-107">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="74598-108">方法</span><span class="sxs-lookup"><span data-stu-id="74598-108">Methods</span></span>
|<span data-ttu-id="74598-109">方法</span><span class="sxs-lookup"><span data-stu-id="74598-109">Method</span></span>|<span data-ttu-id="74598-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="74598-110">Return Type</span></span>|<span data-ttu-id="74598-111">说明</span><span class="sxs-lookup"><span data-stu-id="74598-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74598-112">列出 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="74598-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="74598-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74598-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="74598-114">列出 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74598-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="74598-115">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74598-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="74598-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74598-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="74598-117">读取 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74598-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="74598-118">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74598-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="74598-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74598-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="74598-120">创建新的 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74598-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="74598-121">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74598-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="74598-122">无</span><span class="sxs-lookup"><span data-stu-id="74598-122">None</span></span>|<span data-ttu-id="74598-123">删除 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="74598-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="74598-124">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74598-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="74598-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74598-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="74598-126">更新 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74598-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74598-127">属性</span><span class="sxs-lookup"><span data-stu-id="74598-127">Properties</span></span>
|<span data-ttu-id="74598-128">属性</span><span class="sxs-lookup"><span data-stu-id="74598-128">Property</span></span>|<span data-ttu-id="74598-129">类型</span><span class="sxs-lookup"><span data-stu-id="74598-129">Type</span></span>|<span data-ttu-id="74598-130">说明</span><span class="sxs-lookup"><span data-stu-id="74598-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74598-131">id</span><span class="sxs-lookup"><span data-stu-id="74598-131">id</span></span>|<span data-ttu-id="74598-132">String</span><span class="sxs-lookup"><span data-stu-id="74598-132">String</span></span>|<span data-ttu-id="74598-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74598-133">Key of the entity.</span></span>|
|<span data-ttu-id="74598-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="74598-134">deviceName</span></span>|<span data-ttu-id="74598-135">String</span><span class="sxs-lookup"><span data-stu-id="74598-135">String</span></span>|<span data-ttu-id="74598-136">设备名称</span><span class="sxs-lookup"><span data-stu-id="74598-136">Device name</span></span>|
|<span data-ttu-id="74598-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="74598-137">deviceId</span></span>|<span data-ttu-id="74598-138">String</span><span class="sxs-lookup"><span data-stu-id="74598-138">String</span></span>|<span data-ttu-id="74598-139">设备 ID</span><span class="sxs-lookup"><span data-stu-id="74598-139">Device ID</span></span>|
|<span data-ttu-id="74598-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="74598-140">lastSyncDateTime</span></span>|<span data-ttu-id="74598-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74598-141">DateTimeOffset</span></span>|<span data-ttu-id="74598-142">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="74598-142">Last sync date time</span></span>|
|<span data-ttu-id="74598-143">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="74598-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="74598-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="74598-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="74598-145">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="74598-145">The install state of the app.</span></span> <span data-ttu-id="74598-146">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="74598-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="74598-147">installState</span><span class="sxs-lookup"><span data-stu-id="74598-147">installState</span></span>|[<span data-ttu-id="74598-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="74598-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="74598-149">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="74598-149">The install state of the app.</span></span> <span data-ttu-id="74598-150">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="74598-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="74598-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="74598-151">installStateDetail</span></span>|[<span data-ttu-id="74598-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="74598-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="74598-153">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="74598-153">The install state detail of the app.</span></span> <span data-ttu-id="74598-154">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、 `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` 。</span><span class="sxs-lookup"><span data-stu-id="74598-154">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="74598-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="74598-155">errorCode</span></span>|<span data-ttu-id="74598-156">Int32</span><span class="sxs-lookup"><span data-stu-id="74598-156">Int32</span></span>|<span data-ttu-id="74598-157">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="74598-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="74598-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="74598-158">osVersion</span></span>|<span data-ttu-id="74598-159">String</span><span class="sxs-lookup"><span data-stu-id="74598-159">String</span></span>|<span data-ttu-id="74598-160">OS 版本</span><span class="sxs-lookup"><span data-stu-id="74598-160">OS Version</span></span>|
|<span data-ttu-id="74598-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="74598-161">osDescription</span></span>|<span data-ttu-id="74598-162">String</span><span class="sxs-lookup"><span data-stu-id="74598-162">String</span></span>|<span data-ttu-id="74598-163">OS 说明</span><span class="sxs-lookup"><span data-stu-id="74598-163">OS Description</span></span>|
|<span data-ttu-id="74598-164">userName</span><span class="sxs-lookup"><span data-stu-id="74598-164">userName</span></span>|<span data-ttu-id="74598-165">String</span><span class="sxs-lookup"><span data-stu-id="74598-165">String</span></span>|<span data-ttu-id="74598-166">设备用户名</span><span class="sxs-lookup"><span data-stu-id="74598-166">Device User Name</span></span>|
|<span data-ttu-id="74598-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74598-167">userPrincipalName</span></span>|<span data-ttu-id="74598-168">String</span><span class="sxs-lookup"><span data-stu-id="74598-168">String</span></span>|<span data-ttu-id="74598-169">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="74598-169">User Principal Name</span></span>|
|<span data-ttu-id="74598-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="74598-170">displayVersion</span></span>|<span data-ttu-id="74598-171">String</span><span class="sxs-lookup"><span data-stu-id="74598-171">String</span></span>|<span data-ttu-id="74598-172">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="74598-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="74598-173">关系</span><span class="sxs-lookup"><span data-stu-id="74598-173">Relationships</span></span>
|<span data-ttu-id="74598-174">关系</span><span class="sxs-lookup"><span data-stu-id="74598-174">Relationship</span></span>|<span data-ttu-id="74598-175">类型</span><span class="sxs-lookup"><span data-stu-id="74598-175">Type</span></span>|<span data-ttu-id="74598-176">说明</span><span class="sxs-lookup"><span data-stu-id="74598-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74598-177">应用程序</span><span class="sxs-lookup"><span data-stu-id="74598-177">app</span></span>|[<span data-ttu-id="74598-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="74598-178">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="74598-179">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="74598-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74598-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74598-180">JSON Representation</span></span>
<span data-ttu-id="74598-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74598-181">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```






