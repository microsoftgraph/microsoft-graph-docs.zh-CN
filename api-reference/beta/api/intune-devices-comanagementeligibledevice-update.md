---
title: 更新 comanagementEligibleDevice
description: 更新 comanagementEligibleDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47dd2c3217623ff565fa739dc7d16bd243291561
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158847"
---
# <a name="update-comanagementeligibledevice"></a><span data-ttu-id="6e119-103">更新 comanagementEligibleDevice</span><span class="sxs-lookup"><span data-stu-id="6e119-103">Update comanagementEligibleDevice</span></span>

<span data-ttu-id="6e119-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e119-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e119-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e119-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e119-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e119-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e119-107">更新 [comanagementEligibleDevice 对象](../resources/intune-devices-comanagementeligibledevice.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6e119-107">Update the properties of a [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e119-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e119-108">Prerequisites</span></span>
<span data-ttu-id="6e119-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e119-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e119-111">Permission type</span></span>|<span data-ttu-id="6e119-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e119-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e119-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e119-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e119-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e119-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6e119-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e119-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e119-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e119-116">Not supported.</span></span>|
|<span data-ttu-id="6e119-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e119-117">Application</span></span>|<span data-ttu-id="6e119-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e119-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e119-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e119-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="6e119-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e119-120">Request headers</span></span>
|<span data-ttu-id="6e119-121">标头</span><span class="sxs-lookup"><span data-stu-id="6e119-121">Header</span></span>|<span data-ttu-id="6e119-122">值</span><span class="sxs-lookup"><span data-stu-id="6e119-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e119-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e119-123">Authorization</span></span>|<span data-ttu-id="6e119-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e119-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e119-125">接受</span><span class="sxs-lookup"><span data-stu-id="6e119-125">Accept</span></span>|<span data-ttu-id="6e119-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e119-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e119-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e119-127">Request body</span></span>
<span data-ttu-id="6e119-128">在请求正文中，提供 [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e119-128">In the request body, supply a JSON representation for the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

<span data-ttu-id="6e119-129">下表显示创建 [comanagementEligibleDevice 时所需的属性](../resources/intune-devices-comanagementeligibledevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6e119-129">The following table shows the properties that are required when you create the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).</span></span>

|<span data-ttu-id="6e119-130">属性</span><span class="sxs-lookup"><span data-stu-id="6e119-130">Property</span></span>|<span data-ttu-id="6e119-131">类型</span><span class="sxs-lookup"><span data-stu-id="6e119-131">Type</span></span>|<span data-ttu-id="6e119-132">说明</span><span class="sxs-lookup"><span data-stu-id="6e119-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e119-133">id</span><span class="sxs-lookup"><span data-stu-id="6e119-133">id</span></span>|<span data-ttu-id="6e119-134">String</span><span class="sxs-lookup"><span data-stu-id="6e119-134">String</span></span>|<span data-ttu-id="6e119-135">设备的唯一 ID</span><span class="sxs-lookup"><span data-stu-id="6e119-135">Unique Id for the device</span></span>|
|<span data-ttu-id="6e119-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="6e119-136">deviceName</span></span>|<span data-ttu-id="6e119-137">String</span><span class="sxs-lookup"><span data-stu-id="6e119-137">String</span></span>|<span data-ttu-id="6e119-138">DeviceName</span><span class="sxs-lookup"><span data-stu-id="6e119-138">DeviceName</span></span>|
|<span data-ttu-id="6e119-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="6e119-139">deviceType</span></span>|[<span data-ttu-id="6e119-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="6e119-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6e119-141">DeviceType。</span><span class="sxs-lookup"><span data-stu-id="6e119-141">DeviceType.</span></span> <span data-ttu-id="6e119-142">可能的值是： `desktop` ， ， ， ， ， ， ， `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` ， `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` 。</span><span class="sxs-lookup"><span data-stu-id="6e119-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="6e119-143">clientRegistrationStatus</span><span class="sxs-lookup"><span data-stu-id="6e119-143">clientRegistrationStatus</span></span>|[<span data-ttu-id="6e119-144">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="6e119-144">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="6e119-145">ClientRegistrationStatus。</span><span class="sxs-lookup"><span data-stu-id="6e119-145">ClientRegistrationStatus.</span></span> <span data-ttu-id="6e119-146">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="6e119-146">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="6e119-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="6e119-147">ownerType</span></span>|[<span data-ttu-id="6e119-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="6e119-148">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="6e119-149">OwnerType。</span><span class="sxs-lookup"><span data-stu-id="6e119-149">OwnerType.</span></span> <span data-ttu-id="6e119-150">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="6e119-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="6e119-151">managementAgents</span><span class="sxs-lookup"><span data-stu-id="6e119-151">managementAgents</span></span>|[<span data-ttu-id="6e119-152">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="6e119-152">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="6e119-153">ManagementAgents。</span><span class="sxs-lookup"><span data-stu-id="6e119-153">ManagementAgents.</span></span> <span data-ttu-id="6e119-154">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="6e119-154">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="6e119-155">managementState</span><span class="sxs-lookup"><span data-stu-id="6e119-155">managementState</span></span>|[<span data-ttu-id="6e119-156">managementState</span><span class="sxs-lookup"><span data-stu-id="6e119-156">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="6e119-157">ManagementState。</span><span class="sxs-lookup"><span data-stu-id="6e119-157">ManagementState.</span></span> <span data-ttu-id="6e119-158">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="6e119-158">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="6e119-159">referenceId</span><span class="sxs-lookup"><span data-stu-id="6e119-159">referenceId</span></span>|<span data-ttu-id="6e119-160">String</span><span class="sxs-lookup"><span data-stu-id="6e119-160">String</span></span>|<span data-ttu-id="6e119-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="6e119-161">ReferenceId</span></span>|
|<span data-ttu-id="6e119-162">mdmStatus</span><span class="sxs-lookup"><span data-stu-id="6e119-162">mdmStatus</span></span>|<span data-ttu-id="6e119-163">String</span><span class="sxs-lookup"><span data-stu-id="6e119-163">String</span></span>|<span data-ttu-id="6e119-164">MDMStatus</span><span class="sxs-lookup"><span data-stu-id="6e119-164">MDMStatus</span></span>|
|<span data-ttu-id="6e119-165">osVersion</span><span class="sxs-lookup"><span data-stu-id="6e119-165">osVersion</span></span>|<span data-ttu-id="6e119-166">String</span><span class="sxs-lookup"><span data-stu-id="6e119-166">String</span></span>|<span data-ttu-id="6e119-167">OSVersion</span><span class="sxs-lookup"><span data-stu-id="6e119-167">OSVersion</span></span>|
|<span data-ttu-id="6e119-168">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6e119-168">serialNumber</span></span>|<span data-ttu-id="6e119-169">String</span><span class="sxs-lookup"><span data-stu-id="6e119-169">String</span></span>|<span data-ttu-id="6e119-170">序列号</span><span class="sxs-lookup"><span data-stu-id="6e119-170">SerialNumber</span></span>|
|<span data-ttu-id="6e119-171">manufacturer</span><span class="sxs-lookup"><span data-stu-id="6e119-171">manufacturer</span></span>|<span data-ttu-id="6e119-172">String</span><span class="sxs-lookup"><span data-stu-id="6e119-172">String</span></span>|<span data-ttu-id="6e119-173">制造商</span><span class="sxs-lookup"><span data-stu-id="6e119-173">Manufacturer</span></span>|
|<span data-ttu-id="6e119-174">model</span><span class="sxs-lookup"><span data-stu-id="6e119-174">model</span></span>|<span data-ttu-id="6e119-175">String</span><span class="sxs-lookup"><span data-stu-id="6e119-175">String</span></span>|<span data-ttu-id="6e119-176">模型</span><span class="sxs-lookup"><span data-stu-id="6e119-176">Model</span></span>|
|<span data-ttu-id="6e119-177">osDescription</span><span class="sxs-lookup"><span data-stu-id="6e119-177">osDescription</span></span>|<span data-ttu-id="6e119-178">String</span><span class="sxs-lookup"><span data-stu-id="6e119-178">String</span></span>|<span data-ttu-id="6e119-179">OSDescription</span><span class="sxs-lookup"><span data-stu-id="6e119-179">OSDescription</span></span>|
|<span data-ttu-id="6e119-180">entitySource</span><span class="sxs-lookup"><span data-stu-id="6e119-180">entitySource</span></span>|<span data-ttu-id="6e119-181">Int32</span><span class="sxs-lookup"><span data-stu-id="6e119-181">Int32</span></span>|<span data-ttu-id="6e119-182">EntitySource</span><span class="sxs-lookup"><span data-stu-id="6e119-182">EntitySource</span></span>|
|<span data-ttu-id="6e119-183">userId</span><span class="sxs-lookup"><span data-stu-id="6e119-183">userId</span></span>|<span data-ttu-id="6e119-184">String</span><span class="sxs-lookup"><span data-stu-id="6e119-184">String</span></span>|<span data-ttu-id="6e119-185">UserId</span><span class="sxs-lookup"><span data-stu-id="6e119-185">UserId</span></span>|
|<span data-ttu-id="6e119-186">upn</span><span class="sxs-lookup"><span data-stu-id="6e119-186">upn</span></span>|<span data-ttu-id="6e119-187">String</span><span class="sxs-lookup"><span data-stu-id="6e119-187">String</span></span>|<span data-ttu-id="6e119-188">UPN</span><span class="sxs-lookup"><span data-stu-id="6e119-188">UPN</span></span>|
|<span data-ttu-id="6e119-189">userEmail</span><span class="sxs-lookup"><span data-stu-id="6e119-189">userEmail</span></span>|<span data-ttu-id="6e119-190">String</span><span class="sxs-lookup"><span data-stu-id="6e119-190">String</span></span>|<span data-ttu-id="6e119-191">UserEmail</span><span class="sxs-lookup"><span data-stu-id="6e119-191">UserEmail</span></span>|
|<span data-ttu-id="6e119-192">userName</span><span class="sxs-lookup"><span data-stu-id="6e119-192">userName</span></span>|<span data-ttu-id="6e119-193">String</span><span class="sxs-lookup"><span data-stu-id="6e119-193">String</span></span>|<span data-ttu-id="6e119-194">UserName</span><span class="sxs-lookup"><span data-stu-id="6e119-194">UserName</span></span>|
|<span data-ttu-id="6e119-195">status</span><span class="sxs-lookup"><span data-stu-id="6e119-195">status</span></span>|[<span data-ttu-id="6e119-196">comanagementEligibleType</span><span class="sxs-lookup"><span data-stu-id="6e119-196">comanagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="6e119-197">ComanagementEligibleStatus。</span><span class="sxs-lookup"><span data-stu-id="6e119-197">ComanagementEligibleStatus.</span></span> <span data-ttu-id="6e119-198">可取值为：`comanaged`、`eligible`、`eligibleButNotAzureAdJoined`、`needsOsUpdate`、`ineligible`。</span><span class="sxs-lookup"><span data-stu-id="6e119-198">Possible values are: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span></span>|



## <a name="response"></a><span data-ttu-id="6e119-199">响应</span><span class="sxs-lookup"><span data-stu-id="6e119-199">Response</span></span>
<span data-ttu-id="6e119-200">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e119-200">If successful, this method returns a `200 OK` response code and an updated [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e119-201">示例</span><span class="sxs-lookup"><span data-stu-id="6e119-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e119-202">请求</span><span class="sxs-lookup"><span data-stu-id="6e119-202">Request</span></span>
<span data-ttu-id="6e119-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e119-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
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

### <a name="response"></a><span data-ttu-id="6e119-204">响应</span><span class="sxs-lookup"><span data-stu-id="6e119-204">Response</span></span>
<span data-ttu-id="6e119-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e119-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




