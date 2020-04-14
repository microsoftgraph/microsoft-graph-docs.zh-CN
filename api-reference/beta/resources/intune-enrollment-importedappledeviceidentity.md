---
title: importedAppleDeviceIdentity 资源类型
description: ImportedAppleDeviceIdentity 资源表示导出的 Apple 设备的设备标识。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a316cd1bac5ac84e0249ce0f5e2958b2381a671
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460846"
---
# <a name="importedappledeviceidentity-resource-type"></a><span data-ttu-id="ff3a8-103">importedAppleDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff3a8-103">importedAppleDeviceIdentity resource type</span></span>

<span data-ttu-id="ff3a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff3a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff3a8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff3a8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff3a8-107">ImportedAppleDeviceIdentity 资源表示导出的 Apple 设备的设备标识。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-107">The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device .</span></span>

## <a name="methods"></a><span data-ttu-id="ff3a8-108">方法</span><span class="sxs-lookup"><span data-stu-id="ff3a8-108">Methods</span></span>
|<span data-ttu-id="ff3a8-109">方法</span><span class="sxs-lookup"><span data-stu-id="ff3a8-109">Method</span></span>|<span data-ttu-id="ff3a8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff3a8-110">Return Type</span></span>|<span data-ttu-id="ff3a8-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff3a8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff3a8-112">列出 importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="ff3a8-112">List importedAppleDeviceIdentities</span></span>](../api/intune-enrollment-importedappledeviceidentity-list.md)|<span data-ttu-id="ff3a8-113">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff3a8-113">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="ff3a8-114">列出[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-114">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="ff3a8-115">获取 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff3a8-115">Get importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-get.md)|[<span data-ttu-id="ff3a8-116">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff3a8-116">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="ff3a8-117">读取[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-117">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="ff3a8-118">创建 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff3a8-118">Create importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-create.md)|[<span data-ttu-id="ff3a8-119">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff3a8-119">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="ff3a8-120">创建新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-120">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="ff3a8-121">删除 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff3a8-121">Delete importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-delete.md)|<span data-ttu-id="ff3a8-122">无</span><span class="sxs-lookup"><span data-stu-id="ff3a8-122">None</span></span>|<span data-ttu-id="ff3a8-123">删除[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-123">Deletes a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>|
|[<span data-ttu-id="ff3a8-124">更新 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff3a8-124">Update importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-update.md)|[<span data-ttu-id="ff3a8-125">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff3a8-125">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="ff3a8-126">更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-126">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="ff3a8-127">importAppleDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="ff3a8-127">importAppleDeviceIdentityList action</span></span>](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|<span data-ttu-id="ff3a8-128">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff3a8-128">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection</span></span>|<span data-ttu-id="ff3a8-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ff3a8-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ff3a8-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff3a8-130">Properties</span></span>
|<span data-ttu-id="ff3a8-131">属性</span><span class="sxs-lookup"><span data-stu-id="ff3a8-131">Property</span></span>|<span data-ttu-id="ff3a8-132">类型</span><span class="sxs-lookup"><span data-stu-id="ff3a8-132">Type</span></span>|<span data-ttu-id="ff3a8-133">说明</span><span class="sxs-lookup"><span data-stu-id="ff3a8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff3a8-134">id</span><span class="sxs-lookup"><span data-stu-id="ff3a8-134">id</span></span>|<span data-ttu-id="ff3a8-135">字符串</span><span class="sxs-lookup"><span data-stu-id="ff3a8-135">String</span></span>|<span data-ttu-id="ff3a8-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-136">Key of the entity.</span></span>|
|<span data-ttu-id="ff3a8-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ff3a8-137">serialNumber</span></span>|<span data-ttu-id="ff3a8-138">String</span><span class="sxs-lookup"><span data-stu-id="ff3a8-138">String</span></span>|<span data-ttu-id="ff3a8-139">设备序列号</span><span class="sxs-lookup"><span data-stu-id="ff3a8-139">Device serial number</span></span>|
|<span data-ttu-id="ff3a8-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="ff3a8-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="ff3a8-141">String</span><span class="sxs-lookup"><span data-stu-id="ff3a8-141">String</span></span>|<span data-ttu-id="ff3a8-142">注册配置文件 Id 管理员打算在下次注册时应用到设备</span><span class="sxs-lookup"><span data-stu-id="ff3a8-142">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="ff3a8-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="ff3a8-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="ff3a8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff3a8-144">DateTimeOffset</span></span>|<span data-ttu-id="ff3a8-145">已将时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="ff3a8-145">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="ff3a8-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ff3a8-146">isSupervised</span></span>|<span data-ttu-id="ff3a8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff3a8-147">Boolean</span></span>|<span data-ttu-id="ff3a8-148">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="ff3a8-149">有关详细信息，请参阅：https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="ff3a8-149">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="ff3a8-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ff3a8-150">discoverySource</span></span>|[<span data-ttu-id="ff3a8-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ff3a8-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="ff3a8-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-152">Apple device discovery source.</span></span> <span data-ttu-id="ff3a8-153">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="ff3a8-154">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ff3a8-154">isDeleted</span></span>|<span data-ttu-id="ff3a8-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="ff3a8-155">Boolean</span></span>|<span data-ttu-id="ff3a8-156">指示设备是否已从 Apple Business Manager 中删除</span><span class="sxs-lookup"><span data-stu-id="ff3a8-156">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="ff3a8-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff3a8-157">createdDateTime</span></span>|<span data-ttu-id="ff3a8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff3a8-158">DateTimeOffset</span></span>|<span data-ttu-id="ff3a8-159">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="ff3a8-159">Created Date Time of the device</span></span>|
|<span data-ttu-id="ff3a8-160">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff3a8-160">lastContactedDateTime</span></span>|<span data-ttu-id="ff3a8-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff3a8-161">DateTimeOffset</span></span>|<span data-ttu-id="ff3a8-162">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="ff3a8-162">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="ff3a8-163">description</span><span class="sxs-lookup"><span data-stu-id="ff3a8-163">description</span></span>|<span data-ttu-id="ff3a8-164">String</span><span class="sxs-lookup"><span data-stu-id="ff3a8-164">String</span></span>|<span data-ttu-id="ff3a8-165">设备的说明</span><span class="sxs-lookup"><span data-stu-id="ff3a8-165">The description of the device</span></span>|
|<span data-ttu-id="ff3a8-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ff3a8-166">enrollmentState</span></span>|[<span data-ttu-id="ff3a8-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ff3a8-167">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="ff3a8-168">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-168">The state of the device in Intune.</span></span> <span data-ttu-id="ff3a8-169">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-169">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ff3a8-170">platform</span><span class="sxs-lookup"><span data-stu-id="ff3a8-170">platform</span></span>|[<span data-ttu-id="ff3a8-171">平台</span><span class="sxs-lookup"><span data-stu-id="ff3a8-171">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="ff3a8-172">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-172">The platform of the Device.</span></span> <span data-ttu-id="ff3a8-173">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-173">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff3a8-174">关系</span><span class="sxs-lookup"><span data-stu-id="ff3a8-174">Relationships</span></span>
<span data-ttu-id="ff3a8-175">无</span><span class="sxs-lookup"><span data-stu-id="ff3a8-175">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff3a8-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff3a8-176">JSON Representation</span></span>
<span data-ttu-id="ff3a8-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff3a8-177">Here is a JSON representation of the resource.</span></span>
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
  "isDeleted": true,
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```



