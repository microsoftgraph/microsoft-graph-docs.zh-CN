---
title: mobileAppInstallStatus 资源类型
description: 包含设备的移动应用程序安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cbdafd4d46ba81d53138080a8c5b0c41e73015e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231901"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="9ef58-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ef58-103">mobileAppInstallStatus resource type</span></span>

<span data-ttu-id="9ef58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ef58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ef58-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ef58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ef58-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ef58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef58-107">包含设备的移动应用程序安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="9ef58-107">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="9ef58-108">方法</span><span class="sxs-lookup"><span data-stu-id="9ef58-108">Methods</span></span>
|<span data-ttu-id="9ef58-109">方法</span><span class="sxs-lookup"><span data-stu-id="9ef58-109">Method</span></span>|<span data-ttu-id="9ef58-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ef58-110">Return Type</span></span>|<span data-ttu-id="9ef58-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ef58-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ef58-112">列出 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="9ef58-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="9ef58-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ef58-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="9ef58-114">列出 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ef58-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="9ef58-115">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9ef58-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="9ef58-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9ef58-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="9ef58-117">读取 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ef58-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="9ef58-118">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9ef58-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="9ef58-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9ef58-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="9ef58-120">创建新的 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ef58-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="9ef58-121">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9ef58-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="9ef58-122">无</span><span class="sxs-lookup"><span data-stu-id="9ef58-122">None</span></span>|<span data-ttu-id="9ef58-123">删除 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="9ef58-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="9ef58-124">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9ef58-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="9ef58-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9ef58-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="9ef58-126">更新 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ef58-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ef58-127">属性</span><span class="sxs-lookup"><span data-stu-id="9ef58-127">Properties</span></span>
|<span data-ttu-id="9ef58-128">属性</span><span class="sxs-lookup"><span data-stu-id="9ef58-128">Property</span></span>|<span data-ttu-id="9ef58-129">类型</span><span class="sxs-lookup"><span data-stu-id="9ef58-129">Type</span></span>|<span data-ttu-id="9ef58-130">说明</span><span class="sxs-lookup"><span data-stu-id="9ef58-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef58-131">id</span><span class="sxs-lookup"><span data-stu-id="9ef58-131">id</span></span>|<span data-ttu-id="9ef58-132">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-132">String</span></span>|<span data-ttu-id="9ef58-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ef58-133">Key of the entity.</span></span>|
|<span data-ttu-id="9ef58-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="9ef58-134">deviceName</span></span>|<span data-ttu-id="9ef58-135">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-135">String</span></span>|<span data-ttu-id="9ef58-136">设备名称</span><span class="sxs-lookup"><span data-stu-id="9ef58-136">Device name</span></span>|
|<span data-ttu-id="9ef58-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="9ef58-137">deviceId</span></span>|<span data-ttu-id="9ef58-138">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-138">String</span></span>|<span data-ttu-id="9ef58-139">设备 ID</span><span class="sxs-lookup"><span data-stu-id="9ef58-139">Device ID</span></span>|
|<span data-ttu-id="9ef58-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9ef58-140">lastSyncDateTime</span></span>|<span data-ttu-id="9ef58-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ef58-141">DateTimeOffset</span></span>|<span data-ttu-id="9ef58-142">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="9ef58-142">Last sync date time</span></span>|
|<span data-ttu-id="9ef58-143">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="9ef58-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="9ef58-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="9ef58-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="9ef58-145">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9ef58-145">The install state of the app.</span></span> <span data-ttu-id="9ef58-146">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="9ef58-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="9ef58-147">installState</span><span class="sxs-lookup"><span data-stu-id="9ef58-147">installState</span></span>|[<span data-ttu-id="9ef58-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="9ef58-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="9ef58-149">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9ef58-149">The install state of the app.</span></span> <span data-ttu-id="9ef58-150">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="9ef58-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="9ef58-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="9ef58-151">installStateDetail</span></span>|[<span data-ttu-id="9ef58-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="9ef58-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="9ef58-153">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="9ef58-153">The install state detail of the app.</span></span> <span data-ttu-id="9ef58-154">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、 `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` 。</span><span class="sxs-lookup"><span data-stu-id="9ef58-154">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="9ef58-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="9ef58-155">errorCode</span></span>|<span data-ttu-id="9ef58-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9ef58-156">Int32</span></span>|<span data-ttu-id="9ef58-157">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9ef58-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="9ef58-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="9ef58-158">osVersion</span></span>|<span data-ttu-id="9ef58-159">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-159">String</span></span>|<span data-ttu-id="9ef58-160">OS 版本</span><span class="sxs-lookup"><span data-stu-id="9ef58-160">OS Version</span></span>|
|<span data-ttu-id="9ef58-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="9ef58-161">osDescription</span></span>|<span data-ttu-id="9ef58-162">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-162">String</span></span>|<span data-ttu-id="9ef58-163">OS 说明</span><span class="sxs-lookup"><span data-stu-id="9ef58-163">OS Description</span></span>|
|<span data-ttu-id="9ef58-164">userName</span><span class="sxs-lookup"><span data-stu-id="9ef58-164">userName</span></span>|<span data-ttu-id="9ef58-165">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-165">String</span></span>|<span data-ttu-id="9ef58-166">设备用户名</span><span class="sxs-lookup"><span data-stu-id="9ef58-166">Device User Name</span></span>|
|<span data-ttu-id="9ef58-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9ef58-167">userPrincipalName</span></span>|<span data-ttu-id="9ef58-168">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-168">String</span></span>|<span data-ttu-id="9ef58-169">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9ef58-169">User Principal Name</span></span>|
|<span data-ttu-id="9ef58-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="9ef58-170">displayVersion</span></span>|<span data-ttu-id="9ef58-171">String</span><span class="sxs-lookup"><span data-stu-id="9ef58-171">String</span></span>|<span data-ttu-id="9ef58-172">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="9ef58-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef58-173">关系</span><span class="sxs-lookup"><span data-stu-id="9ef58-173">Relationships</span></span>
|<span data-ttu-id="9ef58-174">关系</span><span class="sxs-lookup"><span data-stu-id="9ef58-174">Relationship</span></span>|<span data-ttu-id="9ef58-175">类型</span><span class="sxs-lookup"><span data-stu-id="9ef58-175">Type</span></span>|<span data-ttu-id="9ef58-176">说明</span><span class="sxs-lookup"><span data-stu-id="9ef58-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef58-177">应用</span><span class="sxs-lookup"><span data-stu-id="9ef58-177">app</span></span>|[<span data-ttu-id="9ef58-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="9ef58-178">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="9ef58-179">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="9ef58-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ef58-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ef58-180">JSON Representation</span></span>
<span data-ttu-id="9ef58-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ef58-181">Here is a JSON representation of the resource.</span></span>
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




