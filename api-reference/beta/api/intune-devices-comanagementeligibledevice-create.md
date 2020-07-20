---
title: 创建 comanagementEligibleDevice
description: 创建新的 comanagementEligibleDevice 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98a57bdd62f292ba118d09c0c3c31f8d43626f99
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792546"
---
# <a name="create-comanagementeligibledevice"></a><span data-ttu-id="e1036-103">创建 comanagementEligibleDevice</span><span class="sxs-lookup"><span data-stu-id="e1036-103">Create comanagementEligibleDevice</span></span>

<span data-ttu-id="e1036-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1036-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1036-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1036-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1036-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1036-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1036-107">创建新的[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1036-107">Create a new [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1036-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e1036-108">Prerequisites</span></span>
<span data-ttu-id="e1036-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1036-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1036-111">Permission type</span></span>|<span data-ttu-id="e1036-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e1036-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1036-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1036-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1036-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1036-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e1036-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1036-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1036-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1036-116">Not supported.</span></span>|
|<span data-ttu-id="e1036-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1036-117">Application</span></span>|<span data-ttu-id="e1036-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1036-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1036-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1036-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a><span data-ttu-id="e1036-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1036-120">Request headers</span></span>
|<span data-ttu-id="e1036-121">标头</span><span class="sxs-lookup"><span data-stu-id="e1036-121">Header</span></span>|<span data-ttu-id="e1036-122">值</span><span class="sxs-lookup"><span data-stu-id="e1036-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1036-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1036-123">Authorization</span></span>|<span data-ttu-id="e1036-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e1036-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1036-125">接受</span><span class="sxs-lookup"><span data-stu-id="e1036-125">Accept</span></span>|<span data-ttu-id="e1036-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1036-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1036-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1036-127">Request body</span></span>
<span data-ttu-id="e1036-128">在请求正文中，提供 comanagementEligibleDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1036-128">In the request body, supply a JSON representation for the comanagementEligibleDevice object.</span></span>

<span data-ttu-id="e1036-129">下表显示创建 comanagementEligibleDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e1036-129">The following table shows the properties that are required when you create the comanagementEligibleDevice.</span></span>

|<span data-ttu-id="e1036-130">属性</span><span class="sxs-lookup"><span data-stu-id="e1036-130">Property</span></span>|<span data-ttu-id="e1036-131">类型</span><span class="sxs-lookup"><span data-stu-id="e1036-131">Type</span></span>|<span data-ttu-id="e1036-132">说明</span><span class="sxs-lookup"><span data-stu-id="e1036-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1036-133">id</span><span class="sxs-lookup"><span data-stu-id="e1036-133">id</span></span>|<span data-ttu-id="e1036-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e1036-134">String</span></span>|<span data-ttu-id="e1036-135">设备的唯一 Id</span><span class="sxs-lookup"><span data-stu-id="e1036-135">Unique Id for the device</span></span>|
|<span data-ttu-id="e1036-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="e1036-136">deviceName</span></span>|<span data-ttu-id="e1036-137">String</span><span class="sxs-lookup"><span data-stu-id="e1036-137">String</span></span>|<span data-ttu-id="e1036-138">DeviceName</span><span class="sxs-lookup"><span data-stu-id="e1036-138">DeviceName</span></span>|
|<span data-ttu-id="e1036-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="e1036-139">deviceType</span></span>|[<span data-ttu-id="e1036-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="e1036-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="e1036-141">DeviceType.</span><span class="sxs-lookup"><span data-stu-id="e1036-141">DeviceType.</span></span> <span data-ttu-id="e1036-142">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="e1036-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e1036-143">clientRegistrationStatus</span><span class="sxs-lookup"><span data-stu-id="e1036-143">clientRegistrationStatus</span></span>|[<span data-ttu-id="e1036-144">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="e1036-144">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="e1036-145">ClientRegistrationStatus.</span><span class="sxs-lookup"><span data-stu-id="e1036-145">ClientRegistrationStatus.</span></span> <span data-ttu-id="e1036-146">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="e1036-146">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="e1036-147">所有者</span><span class="sxs-lookup"><span data-stu-id="e1036-147">ownerType</span></span>|[<span data-ttu-id="e1036-148">所有者</span><span class="sxs-lookup"><span data-stu-id="e1036-148">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="e1036-149">所有者.</span><span class="sxs-lookup"><span data-stu-id="e1036-149">OwnerType.</span></span> <span data-ttu-id="e1036-150">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="e1036-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="e1036-151">managementAgents</span><span class="sxs-lookup"><span data-stu-id="e1036-151">managementAgents</span></span>|[<span data-ttu-id="e1036-152">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="e1036-152">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="e1036-153">ManagementAgents.</span><span class="sxs-lookup"><span data-stu-id="e1036-153">ManagementAgents.</span></span> <span data-ttu-id="e1036-154">可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`windowsManagementCloudApi`。</span><span class="sxs-lookup"><span data-stu-id="e1036-154">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="e1036-155">managementState</span><span class="sxs-lookup"><span data-stu-id="e1036-155">managementState</span></span>|[<span data-ttu-id="e1036-156">managementState</span><span class="sxs-lookup"><span data-stu-id="e1036-156">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="e1036-157">ManagementState.</span><span class="sxs-lookup"><span data-stu-id="e1036-157">ManagementState.</span></span> <span data-ttu-id="e1036-158">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="e1036-158">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="e1036-159">referenceId</span><span class="sxs-lookup"><span data-stu-id="e1036-159">referenceId</span></span>|<span data-ttu-id="e1036-160">String</span><span class="sxs-lookup"><span data-stu-id="e1036-160">String</span></span>|<span data-ttu-id="e1036-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="e1036-161">ReferenceId</span></span>|
|<span data-ttu-id="e1036-162">mdmStatus</span><span class="sxs-lookup"><span data-stu-id="e1036-162">mdmStatus</span></span>|<span data-ttu-id="e1036-163">String</span><span class="sxs-lookup"><span data-stu-id="e1036-163">String</span></span>|<span data-ttu-id="e1036-164">MDMStatus</span><span class="sxs-lookup"><span data-stu-id="e1036-164">MDMStatus</span></span>|
|<span data-ttu-id="e1036-165">osVersion</span><span class="sxs-lookup"><span data-stu-id="e1036-165">osVersion</span></span>|<span data-ttu-id="e1036-166">String</span><span class="sxs-lookup"><span data-stu-id="e1036-166">String</span></span>|<span data-ttu-id="e1036-167">OSVersion</span><span class="sxs-lookup"><span data-stu-id="e1036-167">OSVersion</span></span>|
|<span data-ttu-id="e1036-168">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e1036-168">serialNumber</span></span>|<span data-ttu-id="e1036-169">String</span><span class="sxs-lookup"><span data-stu-id="e1036-169">String</span></span>|<span data-ttu-id="e1036-170">序列号</span><span class="sxs-lookup"><span data-stu-id="e1036-170">SerialNumber</span></span>|
|<span data-ttu-id="e1036-171">manufacturer</span><span class="sxs-lookup"><span data-stu-id="e1036-171">manufacturer</span></span>|<span data-ttu-id="e1036-172">String</span><span class="sxs-lookup"><span data-stu-id="e1036-172">String</span></span>|<span data-ttu-id="e1036-173">负责</span><span class="sxs-lookup"><span data-stu-id="e1036-173">Manufacturer</span></span>|
|<span data-ttu-id="e1036-174">model</span><span class="sxs-lookup"><span data-stu-id="e1036-174">model</span></span>|<span data-ttu-id="e1036-175">String</span><span class="sxs-lookup"><span data-stu-id="e1036-175">String</span></span>|<span data-ttu-id="e1036-176">模型</span><span class="sxs-lookup"><span data-stu-id="e1036-176">Model</span></span>|
|<span data-ttu-id="e1036-177">osDescription</span><span class="sxs-lookup"><span data-stu-id="e1036-177">osDescription</span></span>|<span data-ttu-id="e1036-178">String</span><span class="sxs-lookup"><span data-stu-id="e1036-178">String</span></span>|<span data-ttu-id="e1036-179">OSDescription</span><span class="sxs-lookup"><span data-stu-id="e1036-179">OSDescription</span></span>|
|<span data-ttu-id="e1036-180">entitySource</span><span class="sxs-lookup"><span data-stu-id="e1036-180">entitySource</span></span>|<span data-ttu-id="e1036-181">Int32</span><span class="sxs-lookup"><span data-stu-id="e1036-181">Int32</span></span>|<span data-ttu-id="e1036-182">EntitySource</span><span class="sxs-lookup"><span data-stu-id="e1036-182">EntitySource</span></span>|
|<span data-ttu-id="e1036-183">userId</span><span class="sxs-lookup"><span data-stu-id="e1036-183">userId</span></span>|<span data-ttu-id="e1036-184">String</span><span class="sxs-lookup"><span data-stu-id="e1036-184">String</span></span>|<span data-ttu-id="e1036-185">UserId</span><span class="sxs-lookup"><span data-stu-id="e1036-185">UserId</span></span>|
|<span data-ttu-id="e1036-186">upn</span><span class="sxs-lookup"><span data-stu-id="e1036-186">upn</span></span>|<span data-ttu-id="e1036-187">String</span><span class="sxs-lookup"><span data-stu-id="e1036-187">String</span></span>|<span data-ttu-id="e1036-188">UPN</span><span class="sxs-lookup"><span data-stu-id="e1036-188">UPN</span></span>|
|<span data-ttu-id="e1036-189">userEmail</span><span class="sxs-lookup"><span data-stu-id="e1036-189">userEmail</span></span>|<span data-ttu-id="e1036-190">String</span><span class="sxs-lookup"><span data-stu-id="e1036-190">String</span></span>|<span data-ttu-id="e1036-191">UserEmail</span><span class="sxs-lookup"><span data-stu-id="e1036-191">UserEmail</span></span>|
|<span data-ttu-id="e1036-192">userName</span><span class="sxs-lookup"><span data-stu-id="e1036-192">userName</span></span>|<span data-ttu-id="e1036-193">String</span><span class="sxs-lookup"><span data-stu-id="e1036-193">String</span></span>|<span data-ttu-id="e1036-194">UserName</span><span class="sxs-lookup"><span data-stu-id="e1036-194">UserName</span></span>|
|<span data-ttu-id="e1036-195">status</span><span class="sxs-lookup"><span data-stu-id="e1036-195">status</span></span>|[<span data-ttu-id="e1036-196">comanagementEligibleType</span><span class="sxs-lookup"><span data-stu-id="e1036-196">comanagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="e1036-197">ComanagementEligibleStatus.</span><span class="sxs-lookup"><span data-stu-id="e1036-197">ComanagementEligibleStatus.</span></span> <span data-ttu-id="e1036-198">可取值为：`comanaged`、`eligible`、`eligibleButNotAzureAdJoined`、`needsOsUpdate`、`ineligible`。</span><span class="sxs-lookup"><span data-stu-id="e1036-198">Possible values are: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span></span>|



## <a name="response"></a><span data-ttu-id="e1036-199">响应</span><span class="sxs-lookup"><span data-stu-id="e1036-199">Response</span></span>
<span data-ttu-id="e1036-200">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1036-200">If successful, this method returns a `201 Created` response code and a [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1036-201">示例</span><span class="sxs-lookup"><span data-stu-id="e1036-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1036-202">请求</span><span class="sxs-lookup"><span data-stu-id="e1036-202">Request</span></span>
<span data-ttu-id="e1036-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1036-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices
Content-type: application/json
Content-length: 714

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```

### <a name="response"></a><span data-ttu-id="e1036-204">响应</span><span class="sxs-lookup"><span data-stu-id="e1036-204">Response</span></span>
<span data-ttu-id="e1036-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1036-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```



