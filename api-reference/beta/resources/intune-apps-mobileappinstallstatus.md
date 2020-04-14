---
title: mobileAppInstallStatus 资源类型
description: 包含设备的移动应用程序安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc5ffc7c5dcf1800736b3a2f336069233d29e6a3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440372"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="ec828-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec828-103">mobileAppInstallStatus resource type</span></span>

<span data-ttu-id="ec828-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec828-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec828-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec828-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec828-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec828-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec828-107">包含设备的移动应用程序安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="ec828-107">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="ec828-108">方法</span><span class="sxs-lookup"><span data-stu-id="ec828-108">Methods</span></span>
|<span data-ttu-id="ec828-109">方法</span><span class="sxs-lookup"><span data-stu-id="ec828-109">Method</span></span>|<span data-ttu-id="ec828-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ec828-110">Return Type</span></span>|<span data-ttu-id="ec828-111">说明</span><span class="sxs-lookup"><span data-stu-id="ec828-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec828-112">列出 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="ec828-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="ec828-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="ec828-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="ec828-114">列出[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec828-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="ec828-115">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ec828-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="ec828-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ec828-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="ec828-117">读取[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec828-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="ec828-118">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ec828-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="ec828-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ec828-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="ec828-120">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec828-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="ec828-121">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ec828-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="ec828-122">无</span><span class="sxs-lookup"><span data-stu-id="ec828-122">None</span></span>|<span data-ttu-id="ec828-123">删除[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="ec828-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="ec828-124">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ec828-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="ec828-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ec828-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="ec828-126">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ec828-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec828-127">属性</span><span class="sxs-lookup"><span data-stu-id="ec828-127">Properties</span></span>
|<span data-ttu-id="ec828-128">属性</span><span class="sxs-lookup"><span data-stu-id="ec828-128">Property</span></span>|<span data-ttu-id="ec828-129">类型</span><span class="sxs-lookup"><span data-stu-id="ec828-129">Type</span></span>|<span data-ttu-id="ec828-130">说明</span><span class="sxs-lookup"><span data-stu-id="ec828-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec828-131">id</span><span class="sxs-lookup"><span data-stu-id="ec828-131">id</span></span>|<span data-ttu-id="ec828-132">String</span><span class="sxs-lookup"><span data-stu-id="ec828-132">String</span></span>|<span data-ttu-id="ec828-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec828-133">Key of the entity.</span></span>|
|<span data-ttu-id="ec828-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="ec828-134">deviceName</span></span>|<span data-ttu-id="ec828-135">String</span><span class="sxs-lookup"><span data-stu-id="ec828-135">String</span></span>|<span data-ttu-id="ec828-136">设备名称</span><span class="sxs-lookup"><span data-stu-id="ec828-136">Device name</span></span>|
|<span data-ttu-id="ec828-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="ec828-137">deviceId</span></span>|<span data-ttu-id="ec828-138">String</span><span class="sxs-lookup"><span data-stu-id="ec828-138">String</span></span>|<span data-ttu-id="ec828-139">设备 ID</span><span class="sxs-lookup"><span data-stu-id="ec828-139">Device ID</span></span>|
|<span data-ttu-id="ec828-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec828-140">lastSyncDateTime</span></span>|<span data-ttu-id="ec828-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec828-141">DateTimeOffset</span></span>|<span data-ttu-id="ec828-142">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="ec828-142">Last sync date time</span></span>|
|<span data-ttu-id="ec828-143">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="ec828-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="ec828-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ec828-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ec828-145">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="ec828-145">The install state of the app.</span></span> <span data-ttu-id="ec828-146">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="ec828-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ec828-147">installState</span><span class="sxs-lookup"><span data-stu-id="ec828-147">installState</span></span>|[<span data-ttu-id="ec828-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ec828-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ec828-149">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="ec828-149">The install state of the app.</span></span> <span data-ttu-id="ec828-150">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="ec828-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ec828-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="ec828-151">installStateDetail</span></span>|[<span data-ttu-id="ec828-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="ec828-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="ec828-153">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="ec828-153">The install state detail of the app.</span></span> <span data-ttu-id="ec828-154">可取值为：`noAdditionalDetails`、`dependencyFailedToInstall`、`dependencyWithRequirementsNotMet`、`dependencyPendingReboot`、`dependencyWithAutoInstallDisabled`、`seeInstallErrorCode`、`autoInstallDisabled`、`seeUninstallErrorCode`、`pendingReboot`、`installingDependencies`、`contentDownloaded`、`powerShellScriptRequirementNotMet`、`registryRequirementNotMet`、`fileSystemRequirementNotMet`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="ec828-154">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="ec828-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="ec828-155">errorCode</span></span>|<span data-ttu-id="ec828-156">Int32</span><span class="sxs-lookup"><span data-stu-id="ec828-156">Int32</span></span>|<span data-ttu-id="ec828-157">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ec828-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="ec828-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="ec828-158">osVersion</span></span>|<span data-ttu-id="ec828-159">String</span><span class="sxs-lookup"><span data-stu-id="ec828-159">String</span></span>|<span data-ttu-id="ec828-160">OS 版本</span><span class="sxs-lookup"><span data-stu-id="ec828-160">OS Version</span></span>|
|<span data-ttu-id="ec828-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="ec828-161">osDescription</span></span>|<span data-ttu-id="ec828-162">String</span><span class="sxs-lookup"><span data-stu-id="ec828-162">String</span></span>|<span data-ttu-id="ec828-163">OS 说明</span><span class="sxs-lookup"><span data-stu-id="ec828-163">OS Description</span></span>|
|<span data-ttu-id="ec828-164">userName</span><span class="sxs-lookup"><span data-stu-id="ec828-164">userName</span></span>|<span data-ttu-id="ec828-165">String</span><span class="sxs-lookup"><span data-stu-id="ec828-165">String</span></span>|<span data-ttu-id="ec828-166">设备用户名</span><span class="sxs-lookup"><span data-stu-id="ec828-166">Device User Name</span></span>|
|<span data-ttu-id="ec828-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec828-167">userPrincipalName</span></span>|<span data-ttu-id="ec828-168">String</span><span class="sxs-lookup"><span data-stu-id="ec828-168">String</span></span>|<span data-ttu-id="ec828-169">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ec828-169">User Principal Name</span></span>|
|<span data-ttu-id="ec828-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="ec828-170">displayVersion</span></span>|<span data-ttu-id="ec828-171">String</span><span class="sxs-lookup"><span data-stu-id="ec828-171">String</span></span>|<span data-ttu-id="ec828-172">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="ec828-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec828-173">关系</span><span class="sxs-lookup"><span data-stu-id="ec828-173">Relationships</span></span>
|<span data-ttu-id="ec828-174">关系</span><span class="sxs-lookup"><span data-stu-id="ec828-174">Relationship</span></span>|<span data-ttu-id="ec828-175">类型</span><span class="sxs-lookup"><span data-stu-id="ec828-175">Type</span></span>|<span data-ttu-id="ec828-176">说明</span><span class="sxs-lookup"><span data-stu-id="ec828-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec828-177">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec828-177">app</span></span>|[<span data-ttu-id="ec828-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="ec828-178">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="ec828-179">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="ec828-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec828-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec828-180">JSON Representation</span></span>
<span data-ttu-id="ec828-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec828-181">Here is a JSON representation of the resource.</span></span>
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



