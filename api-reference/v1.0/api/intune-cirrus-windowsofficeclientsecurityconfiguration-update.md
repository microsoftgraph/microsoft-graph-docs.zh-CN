---
title: 更新 windowsOfficeClientSecurityConfiguration
description: 更新 windowsOfficeClientSecurityConfiguration 对象的属性。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bff69df9d66d966caaee82549f4af05609f343ac
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753048"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="ca026-103">更新 windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca026-103">Update windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="ca026-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca026-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca026-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca026-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca026-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca026-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca026-107">更新 [windowsOfficeClientSecurityConfiguration 对象](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ca026-107">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca026-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca026-108">Prerequisites</span></span>
<span data-ttu-id="ca026-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca026-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca026-111">Permission type</span></span>|<span data-ttu-id="ca026-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca026-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca026-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca026-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca026-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca026-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca026-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca026-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca026-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca026-116">Not supported.</span></span>|
|<span data-ttu-id="ca026-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca026-117">Application</span></span>|<span data-ttu-id="ca026-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca026-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca026-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca026-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ca026-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca026-120">Request headers</span></span>
|<span data-ttu-id="ca026-121">标头</span><span class="sxs-lookup"><span data-stu-id="ca026-121">Header</span></span>|<span data-ttu-id="ca026-122">值</span><span class="sxs-lookup"><span data-stu-id="ca026-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca026-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca026-123">Authorization</span></span>|<span data-ttu-id="ca026-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca026-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca026-125">接受</span><span class="sxs-lookup"><span data-stu-id="ca026-125">Accept</span></span>|<span data-ttu-id="ca026-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca026-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca026-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca026-127">Request body</span></span>
<span data-ttu-id="ca026-128">在请求正文中，提供 [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca026-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="ca026-129">下表显示创建 [windowsOfficeClientSecurityConfiguration 时所需的属性](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ca026-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="ca026-130">属性</span><span class="sxs-lookup"><span data-stu-id="ca026-130">Property</span></span>|<span data-ttu-id="ca026-131">类型</span><span class="sxs-lookup"><span data-stu-id="ca026-131">Type</span></span>|<span data-ttu-id="ca026-132">说明</span><span class="sxs-lookup"><span data-stu-id="ca026-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca026-133">id</span><span class="sxs-lookup"><span data-stu-id="ca026-133">id</span></span>|<span data-ttu-id="ca026-134">String</span><span class="sxs-lookup"><span data-stu-id="ca026-134">String</span></span>|<span data-ttu-id="ca026-135">Office 客户端配置策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="ca026-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="ca026-136">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="ca026-137">userPreferencePayload</span></span>|<span data-ttu-id="ca026-138">Stream</span><span class="sxs-lookup"><span data-stu-id="ca026-138">Stream</span></span>|<span data-ttu-id="ca026-139">首选项设置 二进制格式的 JSON 字符串，用户可以替代这些值。</span><span class="sxs-lookup"><span data-stu-id="ca026-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="ca026-140">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="ca026-141">policyPayload</span></span>|<span data-ttu-id="ca026-142">Stream</span><span class="sxs-lookup"><span data-stu-id="ca026-142">Stream</span></span>|<span data-ttu-id="ca026-143">策略设置 二进制格式的 JSON 字符串，用户无法更改这些值。</span><span class="sxs-lookup"><span data-stu-id="ca026-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="ca026-144">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-145">description</span><span class="sxs-lookup"><span data-stu-id="ca026-145">description</span></span>|<span data-ttu-id="ca026-146">String</span><span class="sxs-lookup"><span data-stu-id="ca026-146">String</span></span>|<span data-ttu-id="ca026-147">管理员提供了 Office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ca026-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="ca026-148">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-149">displayName</span><span class="sxs-lookup"><span data-stu-id="ca026-149">displayName</span></span>|<span data-ttu-id="ca026-150">String</span><span class="sxs-lookup"><span data-stu-id="ca026-150">String</span></span>|<span data-ttu-id="ca026-151">管理员提供的 Office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="ca026-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="ca026-152">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-153">assignments</span><span class="sxs-lookup"><span data-stu-id="ca026-153">assignments</span></span>|<span data-ttu-id="ca026-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca026-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ca026-155">策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="ca026-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="ca026-156">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-157">priority</span><span class="sxs-lookup"><span data-stu-id="ca026-157">priority</span></span>|<span data-ttu-id="ca026-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ca026-158">Int32</span></span>|<span data-ttu-id="ca026-159">优先级值应为租户下每个策略的唯一值，并且将用于冲突解决，较低的值表示优先级较高。</span><span class="sxs-lookup"><span data-stu-id="ca026-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="ca026-160">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca026-161">lastModifiedDateTime</span></span>|<span data-ttu-id="ca026-162">日期时间</span><span class="sxs-lookup"><span data-stu-id="ca026-162">DateTime</span></span>|<span data-ttu-id="ca026-163">策略的上次修改日期/时间戳。</span><span class="sxs-lookup"><span data-stu-id="ca026-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="ca026-164">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ca026-165">userCheckinSummary</span></span>|[<span data-ttu-id="ca026-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ca026-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="ca026-167">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="ca026-167">User check-in summary for the policy.</span></span> <span data-ttu-id="ca026-168">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca026-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="ca026-169">checkinStatuses</span></span>|<span data-ttu-id="ca026-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca026-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="ca026-171">Office 客户端签入状态列表。</span><span class="sxs-lookup"><span data-stu-id="ca026-171">List of office Client check-in status.</span></span> <span data-ttu-id="ca026-172">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca026-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ca026-173">响应</span><span class="sxs-lookup"><span data-stu-id="ca026-173">Response</span></span>
<span data-ttu-id="ca026-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca026-174">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca026-175">示例</span><span class="sxs-lookup"><span data-stu-id="ca026-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca026-176">请求</span><span class="sxs-lookup"><span data-stu-id="ca026-176">Request</span></span>
<span data-ttu-id="ca026-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca026-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}
Content-type: application/json
Content-length: 949

{
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ca026-178">响应</span><span class="sxs-lookup"><span data-stu-id="ca026-178">Response</span></span>
<span data-ttu-id="ca026-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca026-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```




