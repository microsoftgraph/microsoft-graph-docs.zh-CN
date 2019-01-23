---
title: mobileAppInstallStatus 资源类型
description: 包含用于设备的移动应用程序的安装状态属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f9ee188190e834016e7dc919c6a2c672d5e22227
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422430"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="f4b58-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4b58-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="f4b58-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f4b58-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4b58-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f4b58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4b58-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4b58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4b58-107">包含用于设备的移动应用程序的安装状态属性。</span><span class="sxs-lookup"><span data-stu-id="f4b58-107">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="f4b58-108">方法</span><span class="sxs-lookup"><span data-stu-id="f4b58-108">Methods</span></span>
|<span data-ttu-id="f4b58-109">方法</span><span class="sxs-lookup"><span data-stu-id="f4b58-109">Method</span></span>|<span data-ttu-id="f4b58-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4b58-110">Return Type</span></span>|<span data-ttu-id="f4b58-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4b58-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4b58-112">列表 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="f4b58-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="f4b58-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4b58-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="f4b58-114">列出属性和[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f4b58-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="f4b58-115">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4b58-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="f4b58-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4b58-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="f4b58-117">读取属性和[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f4b58-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="f4b58-118">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4b58-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="f4b58-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4b58-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="f4b58-120">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4b58-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="f4b58-121">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4b58-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="f4b58-122">无</span><span class="sxs-lookup"><span data-stu-id="f4b58-122">None</span></span>|<span data-ttu-id="f4b58-123">删除[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="f4b58-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="f4b58-124">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4b58-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="f4b58-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4b58-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="f4b58-126">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4b58-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4b58-127">属性</span><span class="sxs-lookup"><span data-stu-id="f4b58-127">Properties</span></span>
|<span data-ttu-id="f4b58-128">属性</span><span class="sxs-lookup"><span data-stu-id="f4b58-128">Property</span></span>|<span data-ttu-id="f4b58-129">类型</span><span class="sxs-lookup"><span data-stu-id="f4b58-129">Type</span></span>|<span data-ttu-id="f4b58-130">说明</span><span class="sxs-lookup"><span data-stu-id="f4b58-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b58-131">id</span><span class="sxs-lookup"><span data-stu-id="f4b58-131">id</span></span>|<span data-ttu-id="f4b58-132">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-132">String</span></span>|<span data-ttu-id="f4b58-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4b58-133">Key of the entity.</span></span>|
|<span data-ttu-id="f4b58-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="f4b58-134">deviceName</span></span>|<span data-ttu-id="f4b58-135">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-135">String</span></span>|<span data-ttu-id="f4b58-136">设备名称</span><span class="sxs-lookup"><span data-stu-id="f4b58-136">Device name</span></span>|
|<span data-ttu-id="f4b58-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="f4b58-137">deviceId</span></span>|<span data-ttu-id="f4b58-138">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-138">String</span></span>|<span data-ttu-id="f4b58-139">设备 ID</span><span class="sxs-lookup"><span data-stu-id="f4b58-139">Device ID</span></span>|
|<span data-ttu-id="f4b58-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f4b58-140">lastSyncDateTime</span></span>|<span data-ttu-id="f4b58-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b58-141">DateTimeOffset</span></span>|<span data-ttu-id="f4b58-142">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="f4b58-142">Last sync date time</span></span>|
|<span data-ttu-id="f4b58-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="f4b58-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="f4b58-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="f4b58-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f4b58-145">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="f4b58-145">The install state of the app.</span></span> <span data-ttu-id="f4b58-146">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="f4b58-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f4b58-147">installState</span><span class="sxs-lookup"><span data-stu-id="f4b58-147">installState</span></span>|[<span data-ttu-id="f4b58-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="f4b58-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f4b58-149">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="f4b58-149">The install state of the app.</span></span> <span data-ttu-id="f4b58-150">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="f4b58-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f4b58-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="f4b58-151">installStateDetail</span></span>|[<span data-ttu-id="f4b58-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="f4b58-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="f4b58-153">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="f4b58-153">The install state detail of the app.</span></span> <span data-ttu-id="f4b58-154">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="f4b58-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="f4b58-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="f4b58-155">errorCode</span></span>|<span data-ttu-id="f4b58-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b58-156">Int32</span></span>|<span data-ttu-id="f4b58-157">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="f4b58-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="f4b58-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="f4b58-158">osVersion</span></span>|<span data-ttu-id="f4b58-159">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-159">String</span></span>|<span data-ttu-id="f4b58-160">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="f4b58-160">OS Version</span></span>|
|<span data-ttu-id="f4b58-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="f4b58-161">osDescription</span></span>|<span data-ttu-id="f4b58-162">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-162">String</span></span>|<span data-ttu-id="f4b58-163">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="f4b58-163">OS Description</span></span>|
|<span data-ttu-id="f4b58-164">userName</span><span class="sxs-lookup"><span data-stu-id="f4b58-164">userName</span></span>|<span data-ttu-id="f4b58-165">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-165">String</span></span>|<span data-ttu-id="f4b58-166">设备用户名</span><span class="sxs-lookup"><span data-stu-id="f4b58-166">Device User Name</span></span>|
|<span data-ttu-id="f4b58-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4b58-167">userPrincipalName</span></span>|<span data-ttu-id="f4b58-168">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-168">String</span></span>|<span data-ttu-id="f4b58-169">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f4b58-169">User Principal Name</span></span>|
|<span data-ttu-id="f4b58-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="f4b58-170">displayVersion</span></span>|<span data-ttu-id="f4b58-171">String</span><span class="sxs-lookup"><span data-stu-id="f4b58-171">String</span></span>|<span data-ttu-id="f4b58-172">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="f4b58-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4b58-173">关系</span><span class="sxs-lookup"><span data-stu-id="f4b58-173">Relationships</span></span>
|<span data-ttu-id="f4b58-174">关系</span><span class="sxs-lookup"><span data-stu-id="f4b58-174">Relationship</span></span>|<span data-ttu-id="f4b58-175">类型</span><span class="sxs-lookup"><span data-stu-id="f4b58-175">Type</span></span>|<span data-ttu-id="f4b58-176">说明</span><span class="sxs-lookup"><span data-stu-id="f4b58-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b58-177">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4b58-177">app</span></span>|[<span data-ttu-id="f4b58-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="f4b58-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="f4b58-179">导航到移动应用程序链接。</span><span class="sxs-lookup"><span data-stu-id="f4b58-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4b58-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4b58-180">JSON Representation</span></span>
<span data-ttu-id="f4b58-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4b58-181">Here is a JSON representation of the resource.</span></span>
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




