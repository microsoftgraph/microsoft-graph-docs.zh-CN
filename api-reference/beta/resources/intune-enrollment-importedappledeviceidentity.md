---
title: importedAppleDeviceIdentity 资源类型
description: ImportedAppleDeviceIdentity 资源表示 Apple 设备的导入的设备标识。
author: tfitzmac
ms.openlocfilehash: 966e384b63026def366ba19ea634d635d77d9083
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317589"
---
# <a name="importedappledeviceidentity-resource-type"></a><span data-ttu-id="c3db3-103">importedAppleDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3db3-103">importedAppleDeviceIdentity resource type</span></span>

> <span data-ttu-id="c3db3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c3db3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3db3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3db3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3db3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c3db3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3db3-107">ImportedAppleDeviceIdentity 资源表示 Apple 设备的导入的设备标识。</span><span class="sxs-lookup"><span data-stu-id="c3db3-107">The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device .</span></span>
## <a name="methods"></a><span data-ttu-id="c3db3-108">方法</span><span class="sxs-lookup"><span data-stu-id="c3db3-108">Methods</span></span>
|<span data-ttu-id="c3db3-109">方法</span><span class="sxs-lookup"><span data-stu-id="c3db3-109">Method</span></span>|<span data-ttu-id="c3db3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3db3-110">Return Type</span></span>|<span data-ttu-id="c3db3-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3db3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3db3-112">列表 importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="c3db3-112">List importedAppleDeviceIdentities</span></span>](../api/intune-enrollment-importedappledeviceidentity-list.md)|<span data-ttu-id="c3db3-113">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3db3-113">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="c3db3-114">列出属性和[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="c3db3-114">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="c3db3-115">获取 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3db3-115">Get importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-get.md)|[<span data-ttu-id="c3db3-116">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3db3-116">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="c3db3-117">读取属性和[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c3db3-117">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="c3db3-118">创建 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3db3-118">Create importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-create.md)|[<span data-ttu-id="c3db3-119">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3db3-119">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="c3db3-120">创建新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c3db3-120">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="c3db3-121">删除 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3db3-121">Delete importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-delete.md)|<span data-ttu-id="c3db3-122">无</span><span class="sxs-lookup"><span data-stu-id="c3db3-122">None</span></span>|<span data-ttu-id="c3db3-123">删除[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="c3db3-123">Deletes a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>|
|[<span data-ttu-id="c3db3-124">更新 importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3db3-124">Update importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-update.md)|[<span data-ttu-id="c3db3-125">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3db3-125">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="c3db3-126">更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3db3-126">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="c3db3-127">importAppleDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="c3db3-127">importAppleDeviceIdentityList action</span></span>](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|<span data-ttu-id="c3db3-128">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3db3-128">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection</span></span>|<span data-ttu-id="c3db3-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c3db3-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c3db3-130">属性</span><span class="sxs-lookup"><span data-stu-id="c3db3-130">Properties</span></span>
|<span data-ttu-id="c3db3-131">属性</span><span class="sxs-lookup"><span data-stu-id="c3db3-131">Property</span></span>|<span data-ttu-id="c3db3-132">类型</span><span class="sxs-lookup"><span data-stu-id="c3db3-132">Type</span></span>|<span data-ttu-id="c3db3-133">说明</span><span class="sxs-lookup"><span data-stu-id="c3db3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3db3-134">id</span><span class="sxs-lookup"><span data-stu-id="c3db3-134">id</span></span>|<span data-ttu-id="c3db3-135">String</span><span class="sxs-lookup"><span data-stu-id="c3db3-135">String</span></span>|<span data-ttu-id="c3db3-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3db3-136">Key of the entity.</span></span>|
|<span data-ttu-id="c3db3-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c3db3-137">serialNumber</span></span>|<span data-ttu-id="c3db3-138">字符串</span><span class="sxs-lookup"><span data-stu-id="c3db3-138">String</span></span>|<span data-ttu-id="c3db3-139">设备序列号</span><span class="sxs-lookup"><span data-stu-id="c3db3-139">Device serial number</span></span>|
|<span data-ttu-id="c3db3-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="c3db3-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="c3db3-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c3db3-141">String</span></span>|<span data-ttu-id="c3db3-142">注册配置文件 Id 管理打算在下一步注册过程适用于设备</span><span class="sxs-lookup"><span data-stu-id="c3db3-142">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="c3db3-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="c3db3-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="c3db3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3db3-144">DateTimeOffset</span></span>|<span data-ttu-id="c3db3-145">时间注册配置文件分配给设备</span><span class="sxs-lookup"><span data-stu-id="c3db3-145">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="c3db3-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c3db3-146">isSupervised</span></span>|<span data-ttu-id="c3db3-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3db3-147">Boolean</span></span>|<span data-ttu-id="c3db3-148">指示是否管理 Apple 设备。</span><span class="sxs-lookup"><span data-stu-id="c3db3-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="c3db3-149">详细信息位于：https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="c3db3-149">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="c3db3-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c3db3-150">discoverySource</span></span>|[<span data-ttu-id="c3db3-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="c3db3-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="c3db3-152">Apple 设备发现源。</span><span class="sxs-lookup"><span data-stu-id="c3db3-152">Apple device discovery source.</span></span> <span data-ttu-id="c3db3-153">可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。</span><span class="sxs-lookup"><span data-stu-id="c3db3-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="c3db3-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3db3-154">createdDateTime</span></span>|<span data-ttu-id="c3db3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3db3-155">DateTimeOffset</span></span>|<span data-ttu-id="c3db3-156">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="c3db3-156">Created Date Time of the device</span></span>|
|<span data-ttu-id="c3db3-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3db3-157">lastContactedDateTime</span></span>|<span data-ttu-id="c3db3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3db3-158">DateTimeOffset</span></span>|<span data-ttu-id="c3db3-159">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="c3db3-159">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="c3db3-160">说明</span><span class="sxs-lookup"><span data-stu-id="c3db3-160">description</span></span>|<span data-ttu-id="c3db3-161">字符串</span><span class="sxs-lookup"><span data-stu-id="c3db3-161">String</span></span>|<span data-ttu-id="c3db3-162">设备的说明</span><span class="sxs-lookup"><span data-stu-id="c3db3-162">The description of the device</span></span>|
|<span data-ttu-id="c3db3-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c3db3-163">enrollmentState</span></span>|[<span data-ttu-id="c3db3-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c3db3-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="c3db3-165">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="c3db3-165">The state of the device in Intune.</span></span> <span data-ttu-id="c3db3-166">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c3db3-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c3db3-167">platform</span><span class="sxs-lookup"><span data-stu-id="c3db3-167">platform</span></span>|[<span data-ttu-id="c3db3-168">平台</span><span class="sxs-lookup"><span data-stu-id="c3db3-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="c3db3-169">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="c3db3-169">The platform of the Device.</span></span> <span data-ttu-id="c3db3-170">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="c3db3-170">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3db3-171">Relationships</span><span class="sxs-lookup"><span data-stu-id="c3db3-171">Relationships</span></span>
<span data-ttu-id="c3db3-172">无</span><span class="sxs-lookup"><span data-stu-id="c3db3-172">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3db3-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3db3-173">JSON Representation</span></span>
<span data-ttu-id="c3db3-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3db3-174">Here is a JSON representation of the resource.</span></span>
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





