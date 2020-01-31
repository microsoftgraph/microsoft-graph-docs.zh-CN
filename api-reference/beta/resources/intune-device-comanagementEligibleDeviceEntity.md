---
title: comanagementEligibleDeviceEntity 资源类型
description: comanagementEligibleDeviceEntity 资源类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5ad068a348eabaceafd9ca736f27cf6fda3218e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636551"
---
# <a name="comanagementeligibledeviceentity-resource-type"></a><span data-ttu-id="84f73-103">comanagementEligibleDeviceEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="84f73-103">comanagementEligibleDeviceEntity resource type</span></span>

> <span data-ttu-id="84f73-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84f73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84f73-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84f73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84f73-106">给定设备的托管设备移动应用配置状态。</span><span class="sxs-lookup"><span data-stu-id="84f73-106">Managed Device Mobile App Configuration State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="84f73-107">方法</span><span class="sxs-lookup"><span data-stu-id="84f73-107">Methods</span></span>
|<span data-ttu-id="84f73-108">方法</span><span class="sxs-lookup"><span data-stu-id="84f73-108">Method</span></span>|<span data-ttu-id="84f73-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="84f73-109">Return Type</span></span>|<span data-ttu-id="84f73-110">说明</span><span class="sxs-lookup"><span data-stu-id="84f73-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84f73-111">列出 comanagementEligibleDeviceEntity</span><span class="sxs-lookup"><span data-stu-id="84f73-111">List comanagementEligibleDeviceEntity</span></span>](../api/intune-device-comanagementEligibleDeviceEntity-list.md)|<span data-ttu-id="84f73-112">[comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md)集合</span><span class="sxs-lookup"><span data-stu-id="84f73-112">[comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md) collection</span></span>|<span data-ttu-id="84f73-113">列出[comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84f73-113">List properties and relationships of the [comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="84f73-114">属性</span><span class="sxs-lookup"><span data-stu-id="84f73-114">Properties</span></span>
|<span data-ttu-id="84f73-115">属性</span><span class="sxs-lookup"><span data-stu-id="84f73-115">Property</span></span>|<span data-ttu-id="84f73-116">类型</span><span class="sxs-lookup"><span data-stu-id="84f73-116">Type</span></span>|<span data-ttu-id="84f73-117">说明</span><span class="sxs-lookup"><span data-stu-id="84f73-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84f73-118">id</span><span class="sxs-lookup"><span data-stu-id="84f73-118">id</span></span>|<span data-ttu-id="84f73-119">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-119">String</span></span>|<span data-ttu-id="84f73-120">EligibleDeviceEntity 的唯一 Id</span><span class="sxs-lookup"><span data-stu-id="84f73-120">Unique Id of the EligibleDeviceEntity</span></span>|
|<span data-ttu-id="84f73-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="84f73-121">deviceId</span></span>|<span data-ttu-id="84f73-122">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-122">String</span></span>|<span data-ttu-id="84f73-123">DeviceId</span><span class="sxs-lookup"><span data-stu-id="84f73-123">DeviceId</span></span>|
|<span data-ttu-id="84f73-124">deviceName</span><span class="sxs-lookup"><span data-stu-id="84f73-124">deviceName</span></span>|<span data-ttu-id="84f73-125">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-125">String</span></span>|<span data-ttu-id="84f73-126">DeviceName</span><span class="sxs-lookup"><span data-stu-id="84f73-126">DeviceName</span></span>|
|<span data-ttu-id="84f73-127">deviceType</span><span class="sxs-lookup"><span data-stu-id="84f73-127">deviceType</span></span>|<span data-ttu-id="84f73-128">String</span><span class="sxs-lookup"><span data-stu-id="84f73-128">String</span></span>|<span data-ttu-id="84f73-129">DeviceType</span><span class="sxs-lookup"><span data-stu-id="84f73-129">DeviceType</span></span>|
|<span data-ttu-id="84f73-130">clientRegistrationStatus</span><span class="sxs-lookup"><span data-stu-id="84f73-130">clientRegistrationStatus</span></span>|[<span data-ttu-id="84f73-131">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="84f73-131">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="84f73-132">ClientRegistrationStatus.</span><span class="sxs-lookup"><span data-stu-id="84f73-132">ClientRegistrationStatus.</span></span> <span data-ttu-id="84f73-133">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="84f73-133">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="84f73-134">所有者</span><span class="sxs-lookup"><span data-stu-id="84f73-134">ownerType</span></span>|[<span data-ttu-id="84f73-135">所有者</span><span class="sxs-lookup"><span data-stu-id="84f73-135">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="84f73-136">所有者.</span><span class="sxs-lookup"><span data-stu-id="84f73-136">OwnerType.</span></span> <span data-ttu-id="84f73-137">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="84f73-137">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="84f73-138">managementAgents</span><span class="sxs-lookup"><span data-stu-id="84f73-138">managementAgents</span></span>|[<span data-ttu-id="84f73-139">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="84f73-139">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="84f73-140">ManagementAgentType.</span><span class="sxs-lookup"><span data-stu-id="84f73-140">ManagementAgentType.</span></span> <span data-ttu-id="84f73-141">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="84f73-141">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="84f73-142">managementState</span><span class="sxs-lookup"><span data-stu-id="84f73-142">managementState</span></span>|[<span data-ttu-id="84f73-143">managementState</span><span class="sxs-lookup"><span data-stu-id="84f73-143">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="84f73-144">ManagementState.</span><span class="sxs-lookup"><span data-stu-id="84f73-144">ManagementState.</span></span> <span data-ttu-id="84f73-145">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="84f73-145">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="84f73-146">referenceId</span><span class="sxs-lookup"><span data-stu-id="84f73-146">referenceId</span></span>|<span data-ttu-id="84f73-147">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-147">String</span></span>|<span data-ttu-id="84f73-148">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="84f73-148">ReferenceId</span></span>|
|<span data-ttu-id="84f73-149">mdmStatus</span><span class="sxs-lookup"><span data-stu-id="84f73-149">mdmStatus</span></span>|<span data-ttu-id="84f73-150">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-150">String</span></span>|<span data-ttu-id="84f73-151">MDMStatus</span><span class="sxs-lookup"><span data-stu-id="84f73-151">MDMStatus</span></span>|
|<span data-ttu-id="84f73-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="84f73-152">osVersion</span></span>|<span data-ttu-id="84f73-153">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-153">String</span></span>|<span data-ttu-id="84f73-154">OSVersion</span><span class="sxs-lookup"><span data-stu-id="84f73-154">OSVersion</span></span>|
|<span data-ttu-id="84f73-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="84f73-155">serialNumber</span></span>|<span data-ttu-id="84f73-156">String</span><span class="sxs-lookup"><span data-stu-id="84f73-156">String</span></span>|<span data-ttu-id="84f73-157">序列号</span><span class="sxs-lookup"><span data-stu-id="84f73-157">SerialNumber</span></span>|
|<span data-ttu-id="84f73-158">manufacturer</span><span class="sxs-lookup"><span data-stu-id="84f73-158">manufacturer</span></span>|<span data-ttu-id="84f73-159">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-159">String</span></span>|<span data-ttu-id="84f73-160">负责</span><span class="sxs-lookup"><span data-stu-id="84f73-160">Manufacturer</span></span>|
|<span data-ttu-id="84f73-161">model</span><span class="sxs-lookup"><span data-stu-id="84f73-161">model</span></span>|<span data-ttu-id="84f73-162">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-162">String</span></span>|<span data-ttu-id="84f73-163">模型</span><span class="sxs-lookup"><span data-stu-id="84f73-163">Model</span></span>|
|<span data-ttu-id="84f73-164">osDescription</span><span class="sxs-lookup"><span data-stu-id="84f73-164">osDescription</span></span>|<span data-ttu-id="84f73-165">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-165">String</span></span>|<span data-ttu-id="84f73-166">OSDescription</span><span class="sxs-lookup"><span data-stu-id="84f73-166">OSDescription</span></span>|
|<span data-ttu-id="84f73-167">entitySource</span><span class="sxs-lookup"><span data-stu-id="84f73-167">entitySource</span></span>|<span data-ttu-id="84f73-168">Int32</span><span class="sxs-lookup"><span data-stu-id="84f73-168">Int32</span></span>|<span data-ttu-id="84f73-169">EntitySource</span><span class="sxs-lookup"><span data-stu-id="84f73-169">EntitySource</span></span>|
|<span data-ttu-id="84f73-170">userId</span><span class="sxs-lookup"><span data-stu-id="84f73-170">userId</span></span>|<span data-ttu-id="84f73-171">String</span><span class="sxs-lookup"><span data-stu-id="84f73-171">String</span></span>|<span data-ttu-id="84f73-172">UserId</span><span class="sxs-lookup"><span data-stu-id="84f73-172">UserId</span></span>|
|<span data-ttu-id="84f73-173">upn</span><span class="sxs-lookup"><span data-stu-id="84f73-173">upn</span></span>|<span data-ttu-id="84f73-174">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-174">String</span></span>|<span data-ttu-id="84f73-175">UPN</span><span class="sxs-lookup"><span data-stu-id="84f73-175">UPN</span></span>|
|<span data-ttu-id="84f73-176">userEmail</span><span class="sxs-lookup"><span data-stu-id="84f73-176">userEmail</span></span>|<span data-ttu-id="84f73-177">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-177">String</span></span>|<span data-ttu-id="84f73-178">UserEmail</span><span class="sxs-lookup"><span data-stu-id="84f73-178">UserEmail</span></span>|
|<span data-ttu-id="84f73-179">userName</span><span class="sxs-lookup"><span data-stu-id="84f73-179">userName</span></span>|<span data-ttu-id="84f73-180">字符串</span><span class="sxs-lookup"><span data-stu-id="84f73-180">String</span></span>|<span data-ttu-id="84f73-181">UserName</span><span class="sxs-lookup"><span data-stu-id="84f73-181">UserName</span></span>|
|<span data-ttu-id="84f73-182">coManageEligibleStatus</span><span class="sxs-lookup"><span data-stu-id="84f73-182">coManageEligibleStatus</span></span>|[<span data-ttu-id="84f73-183">coManagementEligibleType</span><span class="sxs-lookup"><span data-stu-id="84f73-183">coManagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="84f73-184">CoManagementEligibleType.</span><span class="sxs-lookup"><span data-stu-id="84f73-184">CoManagementEligibleType.</span></span> <span data-ttu-id="84f73-185">可取值为：`coManaged`、`eligible`、`eligibleButNotAadJoined`、`needsOSUpdate`。</span><span class="sxs-lookup"><span data-stu-id="84f73-185">Possible values are: `coManaged`, `eligible`, `eligibleButNotAadJoined`, `needsOSUpdate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84f73-186">关系</span><span class="sxs-lookup"><span data-stu-id="84f73-186">Relationships</span></span>
<span data-ttu-id="84f73-187">无</span><span class="sxs-lookup"><span data-stu-id="84f73-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84f73-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84f73-188">JSON Representation</span></span>
<span data-ttu-id="84f73-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84f73-189">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDeviceEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "clientRegistrationStatus": "String",
  "ownerType": "String",
  "managementAgents": "String",
  "managementState": "String",
  "referenceId": "String",
  "mdmStatus": "String",
  "osVersion": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "osDescription": "String",
  "entitySource": 1024,
  "userId": "String",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "coManageEligibleStatus": "String"
}
```

