---
title: 更新 windowsOfficeClientSecurityConfiguration
description: 更新 windowsOfficeClientSecurityConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ff4df803272ef4c3d3ec8f07d553fe7abddbb65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162774"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="de142-103">更新 windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="de142-103">Update windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="de142-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de142-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de142-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de142-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de142-106">更新[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de142-106">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de142-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="de142-107">Prerequisites</span></span>
<span data-ttu-id="de142-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de142-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="de142-110">Permission type</span></span>|<span data-ttu-id="de142-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de142-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de142-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de142-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de142-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de142-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de142-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de142-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de142-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de142-115">Not supported.</span></span>|
|<span data-ttu-id="de142-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="de142-116">Application</span></span>|<span data-ttu-id="de142-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="de142-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de142-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de142-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="de142-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="de142-119">Request headers</span></span>
|<span data-ttu-id="de142-120">标头</span><span class="sxs-lookup"><span data-stu-id="de142-120">Header</span></span>|<span data-ttu-id="de142-121">值</span><span class="sxs-lookup"><span data-stu-id="de142-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de142-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de142-122">Authorization</span></span>|<span data-ttu-id="de142-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de142-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de142-124">Accept</span><span class="sxs-lookup"><span data-stu-id="de142-124">Accept</span></span>|<span data-ttu-id="de142-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de142-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de142-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="de142-126">Request body</span></span>
<span data-ttu-id="de142-127">在请求正文中, 提供[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de142-127">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="de142-128">下表显示创建[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de142-128">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="de142-129">属性</span><span class="sxs-lookup"><span data-stu-id="de142-129">Property</span></span>|<span data-ttu-id="de142-130">类型</span><span class="sxs-lookup"><span data-stu-id="de142-130">Type</span></span>|<span data-ttu-id="de142-131">说明</span><span class="sxs-lookup"><span data-stu-id="de142-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de142-132">id</span><span class="sxs-lookup"><span data-stu-id="de142-132">id</span></span>|<span data-ttu-id="de142-133">String</span><span class="sxs-lookup"><span data-stu-id="de142-133">String</span></span>|<span data-ttu-id="de142-134">office 客户端配置策略的 Id。</span><span class="sxs-lookup"><span data-stu-id="de142-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="de142-135">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="de142-136">userPreferencePayload</span></span>|<span data-ttu-id="de142-137">Stream</span><span class="sxs-lookup"><span data-stu-id="de142-137">Stream</span></span>|<span data-ttu-id="de142-138">首选项设置 JSON string 二进制格式, 则用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="de142-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="de142-139">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="de142-140">policyPayload</span></span>|<span data-ttu-id="de142-141">Stream</span><span class="sxs-lookup"><span data-stu-id="de142-141">Stream</span></span>|<span data-ttu-id="de142-142">策略设置 JSON string 二进制格式, 用户不能更改这些值。</span><span class="sxs-lookup"><span data-stu-id="de142-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="de142-143">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-144">说明</span><span class="sxs-lookup"><span data-stu-id="de142-144">description</span></span>|<span data-ttu-id="de142-145">String</span><span class="sxs-lookup"><span data-stu-id="de142-145">String</span></span>|<span data-ttu-id="de142-146">管理员提供的 office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="de142-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="de142-147">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-148">displayName</span><span class="sxs-lookup"><span data-stu-id="de142-148">displayName</span></span>|<span data-ttu-id="de142-149">String</span><span class="sxs-lookup"><span data-stu-id="de142-149">String</span></span>|<span data-ttu-id="de142-150">管理员提供的 office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="de142-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="de142-151">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-152">assignments</span><span class="sxs-lookup"><span data-stu-id="de142-152">assignments</span></span>|<span data-ttu-id="de142-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="de142-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="de142-154">策略的组分配列表。。</span><span class="sxs-lookup"><span data-stu-id="de142-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="de142-155">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-156">priority</span><span class="sxs-lookup"><span data-stu-id="de142-156">priority</span></span>|<span data-ttu-id="de142-157">Int32</span><span class="sxs-lookup"><span data-stu-id="de142-157">Int32</span></span>|<span data-ttu-id="de142-158">对于租户下的每个策略, 优先级值应为唯一值, 并将用于冲突解决, 较低值意味着优先级较高。</span><span class="sxs-lookup"><span data-stu-id="de142-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="de142-159">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de142-160">lastModifiedDateTime</span></span>|<span data-ttu-id="de142-161">日期/时间</span><span class="sxs-lookup"><span data-stu-id="de142-161">DateTime</span></span>|<span data-ttu-id="de142-162">策略的上次修改日期时间戳。</span><span class="sxs-lookup"><span data-stu-id="de142-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="de142-163">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-164">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="de142-164">userCheckinSummary</span></span>|[<span data-ttu-id="de142-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="de142-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="de142-166">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="de142-166">User check-in summary for the policy.</span></span> <span data-ttu-id="de142-167">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de142-168">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="de142-168">checkinStatuses</span></span>|<span data-ttu-id="de142-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="de142-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="de142-170">office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="de142-170">List of office Client check-in status.</span></span> <span data-ttu-id="de142-171">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de142-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="de142-172">响应</span><span class="sxs-lookup"><span data-stu-id="de142-172">Response</span></span>
<span data-ttu-id="de142-173">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de142-173">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de142-174">示例</span><span class="sxs-lookup"><span data-stu-id="de142-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="de142-175">请求</span><span class="sxs-lookup"><span data-stu-id="de142-175">Request</span></span>
<span data-ttu-id="de142-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de142-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de142-177">响应</span><span class="sxs-lookup"><span data-stu-id="de142-177">Response</span></span>
<span data-ttu-id="de142-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de142-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



