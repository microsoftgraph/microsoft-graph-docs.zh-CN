---
title: importedAppleDeviceIdentity 资源类型
description: ImportedAppleDeviceIdentity 资源表示导出的 Apple 设备的设备标识。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08e9487fc4c3f63399027e0fe40b5c90ba761547
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999162"
---
# <a name="importedappledeviceidentity-resource-type"></a><span data-ttu-id="04ca4-103">importedAppleDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="04ca4-103">importedAppleDeviceIdentity resource type</span></span>

> <span data-ttu-id="04ca4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04ca4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04ca4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04ca4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04ca4-106">ImportedAppleDeviceIdentity 资源表示导出的 Apple 设备的设备标识。</span><span class="sxs-lookup"><span data-stu-id="04ca4-106">The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device .</span></span>

## <a name="methods"></a><span data-ttu-id="04ca4-107">方法</span><span class="sxs-lookup"><span data-stu-id="04ca4-107">Methods</span></span>
|<span data-ttu-id="04ca4-108">方法</span><span class="sxs-lookup"><span data-stu-id="04ca4-108">Method</span></span>|<span data-ttu-id="04ca4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="04ca4-109">Return Type</span></span>|<span data-ttu-id="04ca4-110">说明</span><span class="sxs-lookup"><span data-stu-id="04ca4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="04ca4-111">列出 importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="04ca4-111">List importedAppleDeviceIdentities</span></span>](../api/intune-enrollment-importedappledeviceidentity-list.md)|<span data-ttu-id="04ca4-112">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="04ca4-112">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="04ca4-113">列出[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04ca4-113">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="04ca4-114">获取 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="04ca4-114">Get importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-get.md)|[<span data-ttu-id="04ca4-115">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="04ca4-115">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="04ca4-116">读取[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04ca4-116">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="04ca4-117">创建 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="04ca4-117">Create importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-create.md)|[<span data-ttu-id="04ca4-118">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="04ca4-118">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="04ca4-119">创建新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04ca4-119">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="04ca4-120">删除 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="04ca4-120">Delete importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-delete.md)|<span data-ttu-id="04ca4-121">无</span><span class="sxs-lookup"><span data-stu-id="04ca4-121">None</span></span>|<span data-ttu-id="04ca4-122">删除[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="04ca4-122">Deletes a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>|
|[<span data-ttu-id="04ca4-123">更新 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="04ca4-123">Update importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-update.md)|[<span data-ttu-id="04ca4-124">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="04ca4-124">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="04ca4-125">更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04ca4-125">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="04ca4-126">importAppleDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="04ca4-126">importAppleDeviceIdentityList action</span></span>](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|<span data-ttu-id="04ca4-127">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="04ca4-127">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection</span></span>|<span data-ttu-id="04ca4-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="04ca4-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="04ca4-129">属性</span><span class="sxs-lookup"><span data-stu-id="04ca4-129">Properties</span></span>
|<span data-ttu-id="04ca4-130">属性</span><span class="sxs-lookup"><span data-stu-id="04ca4-130">Property</span></span>|<span data-ttu-id="04ca4-131">类型</span><span class="sxs-lookup"><span data-stu-id="04ca4-131">Type</span></span>|<span data-ttu-id="04ca4-132">说明</span><span class="sxs-lookup"><span data-stu-id="04ca4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04ca4-133">id</span><span class="sxs-lookup"><span data-stu-id="04ca4-133">id</span></span>|<span data-ttu-id="04ca4-134">字符串</span><span class="sxs-lookup"><span data-stu-id="04ca4-134">String</span></span>|<span data-ttu-id="04ca4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="04ca4-135">Key of the entity.</span></span>|
|<span data-ttu-id="04ca4-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="04ca4-136">serialNumber</span></span>|<span data-ttu-id="04ca4-137">String</span><span class="sxs-lookup"><span data-stu-id="04ca4-137">String</span></span>|<span data-ttu-id="04ca4-138">设备序列号</span><span class="sxs-lookup"><span data-stu-id="04ca4-138">Device serial number</span></span>|
|<span data-ttu-id="04ca4-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="04ca4-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="04ca4-140">String</span><span class="sxs-lookup"><span data-stu-id="04ca4-140">String</span></span>|<span data-ttu-id="04ca4-141">注册配置文件 Id 管理员打算在下次注册时应用到设备</span><span class="sxs-lookup"><span data-stu-id="04ca4-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="04ca4-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="04ca4-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="04ca4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04ca4-143">DateTimeOffset</span></span>|<span data-ttu-id="04ca4-144">已将时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="04ca4-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="04ca4-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="04ca4-145">isSupervised</span></span>|<span data-ttu-id="04ca4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="04ca4-146">Boolean</span></span>|<span data-ttu-id="04ca4-147">指示 Apple 设备是否受到监督。</span><span class="sxs-lookup"><span data-stu-id="04ca4-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="04ca4-148">有关详细信息, 请参阅:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="04ca4-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="04ca4-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="04ca4-149">discoverySource</span></span>|[<span data-ttu-id="04ca4-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="04ca4-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="04ca4-151">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="04ca4-151">Apple device discovery source.</span></span> <span data-ttu-id="04ca4-152">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="04ca4-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="04ca4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04ca4-153">createdDateTime</span></span>|<span data-ttu-id="04ca4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04ca4-154">DateTimeOffset</span></span>|<span data-ttu-id="04ca4-155">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="04ca4-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="04ca4-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="04ca4-156">lastContactedDateTime</span></span>|<span data-ttu-id="04ca4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04ca4-157">DateTimeOffset</span></span>|<span data-ttu-id="04ca4-158">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="04ca4-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="04ca4-159">说明</span><span class="sxs-lookup"><span data-stu-id="04ca4-159">description</span></span>|<span data-ttu-id="04ca4-160">String</span><span class="sxs-lookup"><span data-stu-id="04ca4-160">String</span></span>|<span data-ttu-id="04ca4-161">设备的说明</span><span class="sxs-lookup"><span data-stu-id="04ca4-161">The description of the device</span></span>|
|<span data-ttu-id="04ca4-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="04ca4-162">enrollmentState</span></span>|[<span data-ttu-id="04ca4-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="04ca4-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="04ca4-164">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="04ca4-164">The state of the device in Intune.</span></span> <span data-ttu-id="04ca4-165">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="04ca4-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="04ca4-166">platform</span><span class="sxs-lookup"><span data-stu-id="04ca4-166">platform</span></span>|[<span data-ttu-id="04ca4-167">平台</span><span class="sxs-lookup"><span data-stu-id="04ca4-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="04ca4-168">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="04ca4-168">The platform of the Device.</span></span> <span data-ttu-id="04ca4-169">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="04ca4-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04ca4-170">关系</span><span class="sxs-lookup"><span data-stu-id="04ca4-170">Relationships</span></span>
<span data-ttu-id="04ca4-171">无</span><span class="sxs-lookup"><span data-stu-id="04ca4-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04ca4-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04ca4-172">JSON Representation</span></span>
<span data-ttu-id="04ca4-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04ca4-173">Here is a JSON representation of the resource.</span></span>
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





