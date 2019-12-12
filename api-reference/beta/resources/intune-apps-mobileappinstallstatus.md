---
title: mobileAppInstallStatus 资源类型
description: 包含设备的移动应用程序安装状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95d6d694da12fe4615ada0d0a2a19f5d7d992980
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955615"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="e1045-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1045-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="e1045-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1045-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1045-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1045-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1045-106">包含设备的移动应用程序安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="e1045-106">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="e1045-107">方法</span><span class="sxs-lookup"><span data-stu-id="e1045-107">Methods</span></span>
|<span data-ttu-id="e1045-108">方法</span><span class="sxs-lookup"><span data-stu-id="e1045-108">Method</span></span>|<span data-ttu-id="e1045-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e1045-109">Return Type</span></span>|<span data-ttu-id="e1045-110">说明</span><span class="sxs-lookup"><span data-stu-id="e1045-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e1045-111">列出 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="e1045-111">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="e1045-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="e1045-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="e1045-113">列出[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e1045-113">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="e1045-114">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1045-114">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="e1045-115">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1045-115">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e1045-116">读取[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e1045-116">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e1045-117">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1045-117">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="e1045-118">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1045-118">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e1045-119">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1045-119">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e1045-120">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1045-120">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="e1045-121">None</span><span class="sxs-lookup"><span data-stu-id="e1045-121">None</span></span>|<span data-ttu-id="e1045-122">删除[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="e1045-122">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="e1045-123">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1045-123">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="e1045-124">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e1045-124">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e1045-125">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e1045-125">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1045-126">属性</span><span class="sxs-lookup"><span data-stu-id="e1045-126">Properties</span></span>
|<span data-ttu-id="e1045-127">属性</span><span class="sxs-lookup"><span data-stu-id="e1045-127">Property</span></span>|<span data-ttu-id="e1045-128">类型</span><span class="sxs-lookup"><span data-stu-id="e1045-128">Type</span></span>|<span data-ttu-id="e1045-129">说明</span><span class="sxs-lookup"><span data-stu-id="e1045-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1045-130">id</span><span class="sxs-lookup"><span data-stu-id="e1045-130">id</span></span>|<span data-ttu-id="e1045-131">String</span><span class="sxs-lookup"><span data-stu-id="e1045-131">String</span></span>|<span data-ttu-id="e1045-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e1045-132">Key of the entity.</span></span>|
|<span data-ttu-id="e1045-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="e1045-133">deviceName</span></span>|<span data-ttu-id="e1045-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e1045-134">String</span></span>|<span data-ttu-id="e1045-135">设备名称</span><span class="sxs-lookup"><span data-stu-id="e1045-135">Device name</span></span>|
|<span data-ttu-id="e1045-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="e1045-136">deviceId</span></span>|<span data-ttu-id="e1045-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e1045-137">String</span></span>|<span data-ttu-id="e1045-138">设备 ID</span><span class="sxs-lookup"><span data-stu-id="e1045-138">Device ID</span></span>|
|<span data-ttu-id="e1045-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e1045-139">lastSyncDateTime</span></span>|<span data-ttu-id="e1045-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1045-140">DateTimeOffset</span></span>|<span data-ttu-id="e1045-141">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="e1045-141">Last sync date time</span></span>|
|<span data-ttu-id="e1045-142">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="e1045-142">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="e1045-143">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e1045-143">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e1045-144">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e1045-144">The install state of the app.</span></span> <span data-ttu-id="e1045-145">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e1045-145">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e1045-146">installState</span><span class="sxs-lookup"><span data-stu-id="e1045-146">installState</span></span>|[<span data-ttu-id="e1045-147">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e1045-147">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e1045-148">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e1045-148">The install state of the app.</span></span> <span data-ttu-id="e1045-149">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e1045-149">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e1045-150">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="e1045-150">installStateDetail</span></span>|[<span data-ttu-id="e1045-151">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="e1045-151">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="e1045-152">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="e1045-152">The install state detail of the app.</span></span> <span data-ttu-id="e1045-153">可取值为：`noAdditionalDetails`、`dependencyFailedToInstall`、`dependencyWithRequirementsNotMet`、`dependencyPendingReboot`、`dependencyWithAutoInstallDisabled`、`seeInstallErrorCode`、`autoInstallDisabled`、`seeUninstallErrorCode`、`pendingReboot`、`installingDependencies`、`contentDownloaded`、`powerShellScriptRequirementNotMet`、`registryRequirementNotMet`、`fileSystemRequirementNotMet`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e1045-153">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="e1045-154">errorCode</span><span class="sxs-lookup"><span data-stu-id="e1045-154">errorCode</span></span>|<span data-ttu-id="e1045-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e1045-155">Int32</span></span>|<span data-ttu-id="e1045-156">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="e1045-156">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="e1045-157">osVersion</span><span class="sxs-lookup"><span data-stu-id="e1045-157">osVersion</span></span>|<span data-ttu-id="e1045-158">字符串</span><span class="sxs-lookup"><span data-stu-id="e1045-158">String</span></span>|<span data-ttu-id="e1045-159">OS 版本</span><span class="sxs-lookup"><span data-stu-id="e1045-159">OS Version</span></span>|
|<span data-ttu-id="e1045-160">osDescription</span><span class="sxs-lookup"><span data-stu-id="e1045-160">osDescription</span></span>|<span data-ttu-id="e1045-161">字符串</span><span class="sxs-lookup"><span data-stu-id="e1045-161">String</span></span>|<span data-ttu-id="e1045-162">OS 说明</span><span class="sxs-lookup"><span data-stu-id="e1045-162">OS Description</span></span>|
|<span data-ttu-id="e1045-163">userName</span><span class="sxs-lookup"><span data-stu-id="e1045-163">userName</span></span>|<span data-ttu-id="e1045-164">String</span><span class="sxs-lookup"><span data-stu-id="e1045-164">String</span></span>|<span data-ttu-id="e1045-165">设备用户名</span><span class="sxs-lookup"><span data-stu-id="e1045-165">Device User Name</span></span>|
|<span data-ttu-id="e1045-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1045-166">userPrincipalName</span></span>|<span data-ttu-id="e1045-167">字符串</span><span class="sxs-lookup"><span data-stu-id="e1045-167">String</span></span>|<span data-ttu-id="e1045-168">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e1045-168">User Principal Name</span></span>|
|<span data-ttu-id="e1045-169">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e1045-169">displayVersion</span></span>|<span data-ttu-id="e1045-170">字符串</span><span class="sxs-lookup"><span data-stu-id="e1045-170">String</span></span>|<span data-ttu-id="e1045-171">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="e1045-171">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1045-172">关系</span><span class="sxs-lookup"><span data-stu-id="e1045-172">Relationships</span></span>
|<span data-ttu-id="e1045-173">关系</span><span class="sxs-lookup"><span data-stu-id="e1045-173">Relationship</span></span>|<span data-ttu-id="e1045-174">类型</span><span class="sxs-lookup"><span data-stu-id="e1045-174">Type</span></span>|<span data-ttu-id="e1045-175">说明</span><span class="sxs-lookup"><span data-stu-id="e1045-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1045-176">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1045-176">app</span></span>|[<span data-ttu-id="e1045-177">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e1045-177">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="e1045-178">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="e1045-178">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1045-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1045-179">JSON Representation</span></span>
<span data-ttu-id="e1045-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1045-180">Here is a JSON representation of the resource.</span></span>
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



