---
title: mobileAppInstallStatus 资源类型
description: 包含用于设备的移动应用程序的安装状态属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cac5c94f0669f784bf4cdd020448e40799d53915
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982608"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="d015c-103">mobileAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="d015c-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="d015c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d015c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d015c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d015c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d015c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d015c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d015c-107">包含用于设备的移动应用程序的安装状态属性。</span><span class="sxs-lookup"><span data-stu-id="d015c-107">Contains properties for the installation state of a mobile app for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="d015c-108">方法</span><span class="sxs-lookup"><span data-stu-id="d015c-108">Methods</span></span>
|<span data-ttu-id="d015c-109">方法</span><span class="sxs-lookup"><span data-stu-id="d015c-109">Method</span></span>|<span data-ttu-id="d015c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d015c-110">Return Type</span></span>|<span data-ttu-id="d015c-111">说明</span><span class="sxs-lookup"><span data-stu-id="d015c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d015c-112">列表 mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="d015c-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="d015c-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="d015c-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="d015c-114">列出属性和[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d015c-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="d015c-115">获取 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d015c-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="d015c-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d015c-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="d015c-117">读取属性和[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d015c-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="d015c-118">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d015c-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="d015c-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d015c-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="d015c-120">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d015c-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="d015c-121">删除 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d015c-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="d015c-122">无</span><span class="sxs-lookup"><span data-stu-id="d015c-122">None</span></span>|<span data-ttu-id="d015c-123">删除[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="d015c-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="d015c-124">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d015c-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="d015c-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d015c-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="d015c-126">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d015c-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d015c-127">属性</span><span class="sxs-lookup"><span data-stu-id="d015c-127">Properties</span></span>
|<span data-ttu-id="d015c-128">属性</span><span class="sxs-lookup"><span data-stu-id="d015c-128">Property</span></span>|<span data-ttu-id="d015c-129">类型</span><span class="sxs-lookup"><span data-stu-id="d015c-129">Type</span></span>|<span data-ttu-id="d015c-130">说明</span><span class="sxs-lookup"><span data-stu-id="d015c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d015c-131">id</span><span class="sxs-lookup"><span data-stu-id="d015c-131">id</span></span>|<span data-ttu-id="d015c-132">String</span><span class="sxs-lookup"><span data-stu-id="d015c-132">String</span></span>|<span data-ttu-id="d015c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d015c-133">Key of the entity.</span></span>|
|<span data-ttu-id="d015c-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="d015c-134">deviceName</span></span>|<span data-ttu-id="d015c-135">String</span><span class="sxs-lookup"><span data-stu-id="d015c-135">String</span></span>|<span data-ttu-id="d015c-136">设备名称</span><span class="sxs-lookup"><span data-stu-id="d015c-136">Device name</span></span>|
|<span data-ttu-id="d015c-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="d015c-137">deviceId</span></span>|<span data-ttu-id="d015c-138">String</span><span class="sxs-lookup"><span data-stu-id="d015c-138">String</span></span>|<span data-ttu-id="d015c-139">设备 ID</span><span class="sxs-lookup"><span data-stu-id="d015c-139">Device ID</span></span>|
|<span data-ttu-id="d015c-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d015c-140">lastSyncDateTime</span></span>|<span data-ttu-id="d015c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d015c-141">DateTimeOffset</span></span>|<span data-ttu-id="d015c-142">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="d015c-142">Last sync date time</span></span>|
|<span data-ttu-id="d015c-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="d015c-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="d015c-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d015c-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d015c-145">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="d015c-145">The install state of the app.</span></span> <span data-ttu-id="d015c-146">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="d015c-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d015c-147">installState</span><span class="sxs-lookup"><span data-stu-id="d015c-147">installState</span></span>|[<span data-ttu-id="d015c-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d015c-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d015c-149">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="d015c-149">The install state of the app.</span></span> <span data-ttu-id="d015c-150">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="d015c-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d015c-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="d015c-151">installStateDetail</span></span>|[<span data-ttu-id="d015c-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="d015c-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="d015c-153">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="d015c-153">The install state detail of the app.</span></span> <span data-ttu-id="d015c-154">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="d015c-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="d015c-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="d015c-155">errorCode</span></span>|<span data-ttu-id="d015c-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d015c-156">Int32</span></span>|<span data-ttu-id="d015c-157">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="d015c-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="d015c-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="d015c-158">osVersion</span></span>|<span data-ttu-id="d015c-159">String</span><span class="sxs-lookup"><span data-stu-id="d015c-159">String</span></span>|<span data-ttu-id="d015c-160">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="d015c-160">OS Version</span></span>|
|<span data-ttu-id="d015c-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="d015c-161">osDescription</span></span>|<span data-ttu-id="d015c-162">String</span><span class="sxs-lookup"><span data-stu-id="d015c-162">String</span></span>|<span data-ttu-id="d015c-163">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="d015c-163">OS Description</span></span>|
|<span data-ttu-id="d015c-164">userName</span><span class="sxs-lookup"><span data-stu-id="d015c-164">userName</span></span>|<span data-ttu-id="d015c-165">String</span><span class="sxs-lookup"><span data-stu-id="d015c-165">String</span></span>|<span data-ttu-id="d015c-166">设备用户名</span><span class="sxs-lookup"><span data-stu-id="d015c-166">Device User Name</span></span>|
|<span data-ttu-id="d015c-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d015c-167">userPrincipalName</span></span>|<span data-ttu-id="d015c-168">字符串</span><span class="sxs-lookup"><span data-stu-id="d015c-168">String</span></span>|<span data-ttu-id="d015c-169">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d015c-169">User Principal Name</span></span>|
|<span data-ttu-id="d015c-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="d015c-170">displayVersion</span></span>|<span data-ttu-id="d015c-171">字符串</span><span class="sxs-lookup"><span data-stu-id="d015c-171">String</span></span>|<span data-ttu-id="d015c-172">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="d015c-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="d015c-173">Relationships</span><span class="sxs-lookup"><span data-stu-id="d015c-173">Relationships</span></span>
|<span data-ttu-id="d015c-174">关系</span><span class="sxs-lookup"><span data-stu-id="d015c-174">Relationship</span></span>|<span data-ttu-id="d015c-175">类型</span><span class="sxs-lookup"><span data-stu-id="d015c-175">Type</span></span>|<span data-ttu-id="d015c-176">Description</span><span class="sxs-lookup"><span data-stu-id="d015c-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d015c-177">应用程序</span><span class="sxs-lookup"><span data-stu-id="d015c-177">app</span></span>|[<span data-ttu-id="d015c-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="d015c-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="d015c-179">导航到移动应用程序链接。</span><span class="sxs-lookup"><span data-stu-id="d015c-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d015c-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d015c-180">JSON Representation</span></span>
<span data-ttu-id="d015c-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d015c-181">Here is a JSON representation of the resource.</span></span>
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





