---
title: importedAppleDeviceIdentity 资源类型
description: ImportedAppleDeviceIdentity 资源表示 Apple 设备的导入的设备标识。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae0f940614ae8b872891579957e8f86c92342da8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416823"
---
# <a name="importedappledeviceidentity-resource-type"></a><span data-ttu-id="97b5c-103">importedAppleDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="97b5c-103">importedAppleDeviceIdentity resource type</span></span>

> <span data-ttu-id="97b5c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="97b5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97b5c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97b5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97b5c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97b5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97b5c-107">ImportedAppleDeviceIdentity 资源表示 Apple 设备的导入的设备标识。</span><span class="sxs-lookup"><span data-stu-id="97b5c-107">The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device .</span></span>

## <a name="methods"></a><span data-ttu-id="97b5c-108">方法</span><span class="sxs-lookup"><span data-stu-id="97b5c-108">Methods</span></span>
|<span data-ttu-id="97b5c-109">方法</span><span class="sxs-lookup"><span data-stu-id="97b5c-109">Method</span></span>|<span data-ttu-id="97b5c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="97b5c-110">Return Type</span></span>|<span data-ttu-id="97b5c-111">说明</span><span class="sxs-lookup"><span data-stu-id="97b5c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97b5c-112">列表 importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="97b5c-112">List importedAppleDeviceIdentities</span></span>](../api/intune-enrollment-importedappledeviceidentity-list.md)|<span data-ttu-id="97b5c-113">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="97b5c-113">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="97b5c-114">列出属性和[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="97b5c-114">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="97b5c-115">获取 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="97b5c-115">Get importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-get.md)|[<span data-ttu-id="97b5c-116">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="97b5c-116">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="97b5c-117">读取属性和[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="97b5c-117">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="97b5c-118">创建 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="97b5c-118">Create importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-create.md)|[<span data-ttu-id="97b5c-119">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="97b5c-119">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="97b5c-120">创建新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97b5c-120">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="97b5c-121">删除 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="97b5c-121">Delete importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-delete.md)|<span data-ttu-id="97b5c-122">无</span><span class="sxs-lookup"><span data-stu-id="97b5c-122">None</span></span>|<span data-ttu-id="97b5c-123">删除[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="97b5c-123">Deletes a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>|
|[<span data-ttu-id="97b5c-124">更新 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="97b5c-124">Update importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-update.md)|[<span data-ttu-id="97b5c-125">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="97b5c-125">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="97b5c-126">更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97b5c-126">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="97b5c-127">importAppleDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="97b5c-127">importAppleDeviceIdentityList action</span></span>](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|<span data-ttu-id="97b5c-128">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="97b5c-128">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection</span></span>|<span data-ttu-id="97b5c-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97b5c-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="97b5c-130">属性</span><span class="sxs-lookup"><span data-stu-id="97b5c-130">Properties</span></span>
|<span data-ttu-id="97b5c-131">属性</span><span class="sxs-lookup"><span data-stu-id="97b5c-131">Property</span></span>|<span data-ttu-id="97b5c-132">类型</span><span class="sxs-lookup"><span data-stu-id="97b5c-132">Type</span></span>|<span data-ttu-id="97b5c-133">说明</span><span class="sxs-lookup"><span data-stu-id="97b5c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97b5c-134">id</span><span class="sxs-lookup"><span data-stu-id="97b5c-134">id</span></span>|<span data-ttu-id="97b5c-135">String</span><span class="sxs-lookup"><span data-stu-id="97b5c-135">String</span></span>|<span data-ttu-id="97b5c-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="97b5c-136">Key of the entity.</span></span>|
|<span data-ttu-id="97b5c-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="97b5c-137">serialNumber</span></span>|<span data-ttu-id="97b5c-138">String</span><span class="sxs-lookup"><span data-stu-id="97b5c-138">String</span></span>|<span data-ttu-id="97b5c-139">设备序列号</span><span class="sxs-lookup"><span data-stu-id="97b5c-139">Device serial number</span></span>|
|<span data-ttu-id="97b5c-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="97b5c-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="97b5c-141">String</span><span class="sxs-lookup"><span data-stu-id="97b5c-141">String</span></span>|<span data-ttu-id="97b5c-142">注册配置文件 Id 管理打算在下一步注册过程适用于设备</span><span class="sxs-lookup"><span data-stu-id="97b5c-142">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="97b5c-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="97b5c-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="97b5c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97b5c-144">DateTimeOffset</span></span>|<span data-ttu-id="97b5c-145">时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="97b5c-145">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="97b5c-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="97b5c-146">isSupervised</span></span>|<span data-ttu-id="97b5c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="97b5c-147">Boolean</span></span>|<span data-ttu-id="97b5c-148">指示是否管理 Apple 设备。</span><span class="sxs-lookup"><span data-stu-id="97b5c-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="97b5c-149">详细信息位于：https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="97b5c-149">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="97b5c-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="97b5c-150">discoverySource</span></span>|[<span data-ttu-id="97b5c-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="97b5c-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="97b5c-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="97b5c-152">Apple device discovery source.</span></span> <span data-ttu-id="97b5c-153">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="97b5c-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="97b5c-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97b5c-154">createdDateTime</span></span>|<span data-ttu-id="97b5c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97b5c-155">DateTimeOffset</span></span>|<span data-ttu-id="97b5c-156">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="97b5c-156">Created Date Time of the device</span></span>|
|<span data-ttu-id="97b5c-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="97b5c-157">lastContactedDateTime</span></span>|<span data-ttu-id="97b5c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97b5c-158">DateTimeOffset</span></span>|<span data-ttu-id="97b5c-159">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="97b5c-159">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="97b5c-160">说明</span><span class="sxs-lookup"><span data-stu-id="97b5c-160">description</span></span>|<span data-ttu-id="97b5c-161">String</span><span class="sxs-lookup"><span data-stu-id="97b5c-161">String</span></span>|<span data-ttu-id="97b5c-162">设备的说明</span><span class="sxs-lookup"><span data-stu-id="97b5c-162">The description of the device</span></span>|
|<span data-ttu-id="97b5c-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="97b5c-163">enrollmentState</span></span>|[<span data-ttu-id="97b5c-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="97b5c-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="97b5c-165">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="97b5c-165">The state of the device in Intune.</span></span> <span data-ttu-id="97b5c-166">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="97b5c-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="97b5c-167">platform</span><span class="sxs-lookup"><span data-stu-id="97b5c-167">platform</span></span>|[<span data-ttu-id="97b5c-168">平台</span><span class="sxs-lookup"><span data-stu-id="97b5c-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="97b5c-169">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="97b5c-169">The platform of the Device.</span></span> <span data-ttu-id="97b5c-170">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="97b5c-170">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97b5c-171">关系</span><span class="sxs-lookup"><span data-stu-id="97b5c-171">Relationships</span></span>
<span data-ttu-id="97b5c-172">无</span><span class="sxs-lookup"><span data-stu-id="97b5c-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97b5c-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97b5c-173">JSON Representation</span></span>
<span data-ttu-id="97b5c-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97b5c-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




