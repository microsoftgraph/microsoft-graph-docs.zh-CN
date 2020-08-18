---
title: mobileAppInstallStatus 资源类型
description: 包含设备的移动应用程序安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a77d00cf466f391c12749acef5f2a87cb1f21ce
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792567"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="9bae4-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="9bae4-103">mobileAppInstallStatus resource type</span></span>

<span data-ttu-id="9bae4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bae4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bae4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9bae4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bae4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9bae4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bae4-107">包含设备的移动应用程序安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="9bae4-107">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="9bae4-108">方法</span><span class="sxs-lookup"><span data-stu-id="9bae4-108">Methods</span></span>
|<span data-ttu-id="9bae4-109">方法</span><span class="sxs-lookup"><span data-stu-id="9bae4-109">Method</span></span>|<span data-ttu-id="9bae4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9bae4-110">Return Type</span></span>|<span data-ttu-id="9bae4-111">说明</span><span class="sxs-lookup"><span data-stu-id="9bae4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9bae4-112">列出 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="9bae4-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="9bae4-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9bae4-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="9bae4-114">列出 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9bae4-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="9bae4-115">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9bae4-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="9bae4-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9bae4-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="9bae4-117">读取 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9bae4-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="9bae4-118">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9bae4-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="9bae4-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9bae4-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="9bae4-120">创建新的 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bae4-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="9bae4-121">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9bae4-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="9bae4-122">无</span><span class="sxs-lookup"><span data-stu-id="9bae4-122">None</span></span>|<span data-ttu-id="9bae4-123">删除 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="9bae4-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="9bae4-124">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9bae4-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="9bae4-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9bae4-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="9bae4-126">更新 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9bae4-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9bae4-127">属性</span><span class="sxs-lookup"><span data-stu-id="9bae4-127">Properties</span></span>
|<span data-ttu-id="9bae4-128">属性</span><span class="sxs-lookup"><span data-stu-id="9bae4-128">Property</span></span>|<span data-ttu-id="9bae4-129">类型</span><span class="sxs-lookup"><span data-stu-id="9bae4-129">Type</span></span>|<span data-ttu-id="9bae4-130">说明</span><span class="sxs-lookup"><span data-stu-id="9bae4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bae4-131">id</span><span class="sxs-lookup"><span data-stu-id="9bae4-131">id</span></span>|<span data-ttu-id="9bae4-132">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-132">String</span></span>|<span data-ttu-id="9bae4-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9bae4-133">Key of the entity.</span></span>|
|<span data-ttu-id="9bae4-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="9bae4-134">deviceName</span></span>|<span data-ttu-id="9bae4-135">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-135">String</span></span>|<span data-ttu-id="9bae4-136">设备名称</span><span class="sxs-lookup"><span data-stu-id="9bae4-136">Device name</span></span>|
|<span data-ttu-id="9bae4-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="9bae4-137">deviceId</span></span>|<span data-ttu-id="9bae4-138">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-138">String</span></span>|<span data-ttu-id="9bae4-139">设备 ID</span><span class="sxs-lookup"><span data-stu-id="9bae4-139">Device ID</span></span>|
|<span data-ttu-id="9bae4-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9bae4-140">lastSyncDateTime</span></span>|<span data-ttu-id="9bae4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bae4-141">DateTimeOffset</span></span>|<span data-ttu-id="9bae4-142">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="9bae4-142">Last sync date time</span></span>|
|<span data-ttu-id="9bae4-143">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="9bae4-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="9bae4-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="9bae4-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="9bae4-145">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9bae4-145">The install state of the app.</span></span> <span data-ttu-id="9bae4-146">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="9bae4-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="9bae4-147">installState</span><span class="sxs-lookup"><span data-stu-id="9bae4-147">installState</span></span>|[<span data-ttu-id="9bae4-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="9bae4-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="9bae4-149">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9bae4-149">The install state of the app.</span></span> <span data-ttu-id="9bae4-150">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="9bae4-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="9bae4-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="9bae4-151">installStateDetail</span></span>|[<span data-ttu-id="9bae4-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="9bae4-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="9bae4-153">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="9bae4-153">The install state detail of the app.</span></span> <span data-ttu-id="9bae4-154">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、 `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` 。</span><span class="sxs-lookup"><span data-stu-id="9bae4-154">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="9bae4-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="9bae4-155">errorCode</span></span>|<span data-ttu-id="9bae4-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9bae4-156">Int32</span></span>|<span data-ttu-id="9bae4-157">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9bae4-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="9bae4-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="9bae4-158">osVersion</span></span>|<span data-ttu-id="9bae4-159">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-159">String</span></span>|<span data-ttu-id="9bae4-160">OS 版本</span><span class="sxs-lookup"><span data-stu-id="9bae4-160">OS Version</span></span>|
|<span data-ttu-id="9bae4-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="9bae4-161">osDescription</span></span>|<span data-ttu-id="9bae4-162">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-162">String</span></span>|<span data-ttu-id="9bae4-163">OS 说明</span><span class="sxs-lookup"><span data-stu-id="9bae4-163">OS Description</span></span>|
|<span data-ttu-id="9bae4-164">userName</span><span class="sxs-lookup"><span data-stu-id="9bae4-164">userName</span></span>|<span data-ttu-id="9bae4-165">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-165">String</span></span>|<span data-ttu-id="9bae4-166">设备用户名</span><span class="sxs-lookup"><span data-stu-id="9bae4-166">Device User Name</span></span>|
|<span data-ttu-id="9bae4-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9bae4-167">userPrincipalName</span></span>|<span data-ttu-id="9bae4-168">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-168">String</span></span>|<span data-ttu-id="9bae4-169">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9bae4-169">User Principal Name</span></span>|
|<span data-ttu-id="9bae4-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="9bae4-170">displayVersion</span></span>|<span data-ttu-id="9bae4-171">String</span><span class="sxs-lookup"><span data-stu-id="9bae4-171">String</span></span>|<span data-ttu-id="9bae4-172">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="9bae4-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bae4-173">关系</span><span class="sxs-lookup"><span data-stu-id="9bae4-173">Relationships</span></span>
|<span data-ttu-id="9bae4-174">关系</span><span class="sxs-lookup"><span data-stu-id="9bae4-174">Relationship</span></span>|<span data-ttu-id="9bae4-175">类型</span><span class="sxs-lookup"><span data-stu-id="9bae4-175">Type</span></span>|<span data-ttu-id="9bae4-176">说明</span><span class="sxs-lookup"><span data-stu-id="9bae4-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bae4-177">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bae4-177">app</span></span>|[<span data-ttu-id="9bae4-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="9bae4-178">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="9bae4-179">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="9bae4-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9bae4-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9bae4-180">JSON Representation</span></span>
<span data-ttu-id="9bae4-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bae4-181">Here is a JSON representation of the resource.</span></span>
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



