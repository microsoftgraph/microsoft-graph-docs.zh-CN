---
title: mobileAppInstallStatus 资源类型
description: 包含用于设备的移动应用程序的安装状态属性。
ms.openlocfilehash: efd5969e2c00d0230d8efeddff3c41bac90fe9c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043514"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="e33d5-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="e33d5-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="e33d5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e33d5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e33d5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e33d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e33d5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e33d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e33d5-107">包含用于设备的移动应用程序的安装状态属性。</span><span class="sxs-lookup"><span data-stu-id="e33d5-107">Contains properties for the installation state of a mobile app for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="e33d5-108">方法</span><span class="sxs-lookup"><span data-stu-id="e33d5-108">Methods</span></span>
|<span data-ttu-id="e33d5-109">方法</span><span class="sxs-lookup"><span data-stu-id="e33d5-109">Method</span></span>|<span data-ttu-id="e33d5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e33d5-110">Return Type</span></span>|<span data-ttu-id="e33d5-111">说明</span><span class="sxs-lookup"><span data-stu-id="e33d5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e33d5-112">列表 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="e33d5-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="e33d5-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="e33d5-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="e33d5-114">列出属性和[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e33d5-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="e33d5-115">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e33d5-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="e33d5-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e33d5-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e33d5-117">读取属性和[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e33d5-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e33d5-118">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e33d5-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="e33d5-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e33d5-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e33d5-120">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e33d5-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e33d5-121">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e33d5-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="e33d5-122">无</span><span class="sxs-lookup"><span data-stu-id="e33d5-122">None</span></span>|<span data-ttu-id="e33d5-123">删除[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="e33d5-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="e33d5-124">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e33d5-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="e33d5-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e33d5-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e33d5-126">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e33d5-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e33d5-127">属性</span><span class="sxs-lookup"><span data-stu-id="e33d5-127">Properties</span></span>
|<span data-ttu-id="e33d5-128">属性</span><span class="sxs-lookup"><span data-stu-id="e33d5-128">Property</span></span>|<span data-ttu-id="e33d5-129">类型</span><span class="sxs-lookup"><span data-stu-id="e33d5-129">Type</span></span>|<span data-ttu-id="e33d5-130">说明</span><span class="sxs-lookup"><span data-stu-id="e33d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e33d5-131">id</span><span class="sxs-lookup"><span data-stu-id="e33d5-131">id</span></span>|<span data-ttu-id="e33d5-132">String</span><span class="sxs-lookup"><span data-stu-id="e33d5-132">String</span></span>|<span data-ttu-id="e33d5-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e33d5-133">Key of the entity.</span></span>|
|<span data-ttu-id="e33d5-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="e33d5-134">deviceName</span></span>|<span data-ttu-id="e33d5-135">String</span><span class="sxs-lookup"><span data-stu-id="e33d5-135">String</span></span>|<span data-ttu-id="e33d5-136">设备名称</span><span class="sxs-lookup"><span data-stu-id="e33d5-136">Device name</span></span>|
|<span data-ttu-id="e33d5-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="e33d5-137">deviceId</span></span>|<span data-ttu-id="e33d5-138">String</span><span class="sxs-lookup"><span data-stu-id="e33d5-138">String</span></span>|<span data-ttu-id="e33d5-139">设备 ID</span><span class="sxs-lookup"><span data-stu-id="e33d5-139">Device ID</span></span>|
|<span data-ttu-id="e33d5-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e33d5-140">lastSyncDateTime</span></span>|<span data-ttu-id="e33d5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33d5-141">DateTimeOffset</span></span>|<span data-ttu-id="e33d5-142">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="e33d5-142">Last sync date time</span></span>|
|<span data-ttu-id="e33d5-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="e33d5-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="e33d5-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e33d5-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e33d5-145">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e33d5-145">The install state of the app.</span></span> <span data-ttu-id="e33d5-146">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e33d5-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e33d5-147">installState</span><span class="sxs-lookup"><span data-stu-id="e33d5-147">installState</span></span>|[<span data-ttu-id="e33d5-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e33d5-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e33d5-149">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e33d5-149">The install state of the app.</span></span> <span data-ttu-id="e33d5-150">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e33d5-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e33d5-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="e33d5-151">installStateDetail</span></span>|[<span data-ttu-id="e33d5-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="e33d5-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="e33d5-153">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="e33d5-153">The install state detail of the app.</span></span> <span data-ttu-id="e33d5-154">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e33d5-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="e33d5-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="e33d5-155">errorCode</span></span>|<span data-ttu-id="e33d5-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e33d5-156">Int32</span></span>|<span data-ttu-id="e33d5-157">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="e33d5-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="e33d5-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="e33d5-158">osVersion</span></span>|<span data-ttu-id="e33d5-159">String</span><span class="sxs-lookup"><span data-stu-id="e33d5-159">String</span></span>|<span data-ttu-id="e33d5-160">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="e33d5-160">OS Version</span></span>|
|<span data-ttu-id="e33d5-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="e33d5-161">osDescription</span></span>|<span data-ttu-id="e33d5-162">String</span><span class="sxs-lookup"><span data-stu-id="e33d5-162">String</span></span>|<span data-ttu-id="e33d5-163">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="e33d5-163">OS Description</span></span>|
|<span data-ttu-id="e33d5-164">userName</span><span class="sxs-lookup"><span data-stu-id="e33d5-164">userName</span></span>|<span data-ttu-id="e33d5-165">String</span><span class="sxs-lookup"><span data-stu-id="e33d5-165">String</span></span>|<span data-ttu-id="e33d5-166">设备用户名</span><span class="sxs-lookup"><span data-stu-id="e33d5-166">Device User Name</span></span>|
|<span data-ttu-id="e33d5-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e33d5-167">userPrincipalName</span></span>|<span data-ttu-id="e33d5-168">字符串</span><span class="sxs-lookup"><span data-stu-id="e33d5-168">String</span></span>|<span data-ttu-id="e33d5-169">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e33d5-169">User Principal Name</span></span>|
|<span data-ttu-id="e33d5-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e33d5-170">displayVersion</span></span>|<span data-ttu-id="e33d5-171">字符串</span><span class="sxs-lookup"><span data-stu-id="e33d5-171">String</span></span>|<span data-ttu-id="e33d5-172">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="e33d5-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e33d5-173">Relationships</span><span class="sxs-lookup"><span data-stu-id="e33d5-173">Relationships</span></span>
|<span data-ttu-id="e33d5-174">关系</span><span class="sxs-lookup"><span data-stu-id="e33d5-174">Relationship</span></span>|<span data-ttu-id="e33d5-175">类型</span><span class="sxs-lookup"><span data-stu-id="e33d5-175">Type</span></span>|<span data-ttu-id="e33d5-176">说明</span><span class="sxs-lookup"><span data-stu-id="e33d5-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e33d5-177">应用程序</span><span class="sxs-lookup"><span data-stu-id="e33d5-177">app</span></span>|[<span data-ttu-id="e33d5-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e33d5-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e33d5-179">导航到移动应用程序链接。</span><span class="sxs-lookup"><span data-stu-id="e33d5-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e33d5-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e33d5-180">JSON Representation</span></span>
<span data-ttu-id="e33d5-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e33d5-181">Here is a JSON representation of the resource.</span></span>
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





