---
title: mobileAppInstallStatus 资源类型
description: 包含设备的移动应用程序安装状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5bedb9308b414c4ea44c814c40dcd32ca33074d1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322623"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="6cb25-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="6cb25-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="6cb25-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6cb25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cb25-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6cb25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cb25-106">包含设备的移动应用程序安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="6cb25-106">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="6cb25-107">方法</span><span class="sxs-lookup"><span data-stu-id="6cb25-107">Methods</span></span>
|<span data-ttu-id="6cb25-108">方法</span><span class="sxs-lookup"><span data-stu-id="6cb25-108">Method</span></span>|<span data-ttu-id="6cb25-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6cb25-109">Return Type</span></span>|<span data-ttu-id="6cb25-110">说明</span><span class="sxs-lookup"><span data-stu-id="6cb25-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6cb25-111">列出 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="6cb25-111">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="6cb25-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="6cb25-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="6cb25-113">列出[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6cb25-113">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="6cb25-114">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6cb25-114">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="6cb25-115">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6cb25-115">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="6cb25-116">读取[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6cb25-116">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="6cb25-117">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6cb25-117">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="6cb25-118">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6cb25-118">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="6cb25-119">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6cb25-119">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="6cb25-120">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6cb25-120">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="6cb25-121">无</span><span class="sxs-lookup"><span data-stu-id="6cb25-121">None</span></span>|<span data-ttu-id="6cb25-122">删除[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="6cb25-122">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="6cb25-123">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6cb25-123">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="6cb25-124">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6cb25-124">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="6cb25-125">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6cb25-125">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6cb25-126">属性</span><span class="sxs-lookup"><span data-stu-id="6cb25-126">Properties</span></span>
|<span data-ttu-id="6cb25-127">属性</span><span class="sxs-lookup"><span data-stu-id="6cb25-127">Property</span></span>|<span data-ttu-id="6cb25-128">类型</span><span class="sxs-lookup"><span data-stu-id="6cb25-128">Type</span></span>|<span data-ttu-id="6cb25-129">说明</span><span class="sxs-lookup"><span data-stu-id="6cb25-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cb25-130">id</span><span class="sxs-lookup"><span data-stu-id="6cb25-130">id</span></span>|<span data-ttu-id="6cb25-131">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-131">String</span></span>|<span data-ttu-id="6cb25-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6cb25-132">Key of the entity.</span></span>|
|<span data-ttu-id="6cb25-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="6cb25-133">deviceName</span></span>|<span data-ttu-id="6cb25-134">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-134">String</span></span>|<span data-ttu-id="6cb25-135">设备名称</span><span class="sxs-lookup"><span data-stu-id="6cb25-135">Device name</span></span>|
|<span data-ttu-id="6cb25-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="6cb25-136">deviceId</span></span>|<span data-ttu-id="6cb25-137">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-137">String</span></span>|<span data-ttu-id="6cb25-138">设备 ID</span><span class="sxs-lookup"><span data-stu-id="6cb25-138">Device ID</span></span>|
|<span data-ttu-id="6cb25-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6cb25-139">lastSyncDateTime</span></span>|<span data-ttu-id="6cb25-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cb25-140">DateTimeOffset</span></span>|<span data-ttu-id="6cb25-141">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="6cb25-141">Last sync date time</span></span>|
|<span data-ttu-id="6cb25-142">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="6cb25-142">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="6cb25-143">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="6cb25-143">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="6cb25-144">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="6cb25-144">The install state of the app.</span></span> <span data-ttu-id="6cb25-145">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="6cb25-145">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="6cb25-146">installState</span><span class="sxs-lookup"><span data-stu-id="6cb25-146">installState</span></span>|[<span data-ttu-id="6cb25-147">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="6cb25-147">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="6cb25-148">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="6cb25-148">The install state of the app.</span></span> <span data-ttu-id="6cb25-149">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="6cb25-149">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="6cb25-150">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="6cb25-150">installStateDetail</span></span>|[<span data-ttu-id="6cb25-151">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="6cb25-151">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="6cb25-152">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="6cb25-152">The install state detail of the app.</span></span> <span data-ttu-id="6cb25-153">可能的值为`noAdditionalDetails`: `dependencyFailedToInstall`、 `dependencyWithRequirementsNotMet`、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`、、、、、、、、、、、、、、、、 `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="6cb25-153">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="6cb25-154">errorCode</span><span class="sxs-lookup"><span data-stu-id="6cb25-154">errorCode</span></span>|<span data-ttu-id="6cb25-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb25-155">Int32</span></span>|<span data-ttu-id="6cb25-156">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="6cb25-156">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="6cb25-157">osVersion</span><span class="sxs-lookup"><span data-stu-id="6cb25-157">osVersion</span></span>|<span data-ttu-id="6cb25-158">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-158">String</span></span>|<span data-ttu-id="6cb25-159">OS 版本</span><span class="sxs-lookup"><span data-stu-id="6cb25-159">OS Version</span></span>|
|<span data-ttu-id="6cb25-160">osDescription</span><span class="sxs-lookup"><span data-stu-id="6cb25-160">osDescription</span></span>|<span data-ttu-id="6cb25-161">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-161">String</span></span>|<span data-ttu-id="6cb25-162">OS 说明</span><span class="sxs-lookup"><span data-stu-id="6cb25-162">OS Description</span></span>|
|<span data-ttu-id="6cb25-163">userName</span><span class="sxs-lookup"><span data-stu-id="6cb25-163">userName</span></span>|<span data-ttu-id="6cb25-164">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-164">String</span></span>|<span data-ttu-id="6cb25-165">设备用户名</span><span class="sxs-lookup"><span data-stu-id="6cb25-165">Device User Name</span></span>|
|<span data-ttu-id="6cb25-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6cb25-166">userPrincipalName</span></span>|<span data-ttu-id="6cb25-167">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-167">String</span></span>|<span data-ttu-id="6cb25-168">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="6cb25-168">User Principal Name</span></span>|
|<span data-ttu-id="6cb25-169">displayVersion</span><span class="sxs-lookup"><span data-stu-id="6cb25-169">displayVersion</span></span>|<span data-ttu-id="6cb25-170">String</span><span class="sxs-lookup"><span data-stu-id="6cb25-170">String</span></span>|<span data-ttu-id="6cb25-171">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="6cb25-171">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cb25-172">关系</span><span class="sxs-lookup"><span data-stu-id="6cb25-172">Relationships</span></span>
|<span data-ttu-id="6cb25-173">关系</span><span class="sxs-lookup"><span data-stu-id="6cb25-173">Relationship</span></span>|<span data-ttu-id="6cb25-174">类型</span><span class="sxs-lookup"><span data-stu-id="6cb25-174">Type</span></span>|<span data-ttu-id="6cb25-175">说明</span><span class="sxs-lookup"><span data-stu-id="6cb25-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cb25-176">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cb25-176">app</span></span>|[<span data-ttu-id="6cb25-177">mobileApp</span><span class="sxs-lookup"><span data-stu-id="6cb25-177">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="6cb25-178">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="6cb25-178">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cb25-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6cb25-179">JSON Representation</span></span>
<span data-ttu-id="6cb25-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6cb25-180">Here is a JSON representation of the resource.</span></span>
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



