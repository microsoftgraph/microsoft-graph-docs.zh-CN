---
title: 更新 windowsOfficeClientSecurityConfiguration
description: 更新 windowsOfficeClientSecurityConfiguration 对象的属性。
ms.openlocfilehash: 4e3430250a8b4332e07f9e6548c743aa122e1b19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044843"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="7af1e-103">更新 windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="7af1e-103">Update windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="7af1e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7af1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7af1e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7af1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7af1e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7af1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7af1e-107">更新[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7af1e-107">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7af1e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7af1e-108">Prerequisites</span></span>
<span data-ttu-id="7af1e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7af1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7af1e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7af1e-111">Permission type</span></span>|<span data-ttu-id="7af1e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7af1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7af1e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7af1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7af1e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7af1e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7af1e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7af1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7af1e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7af1e-116">Not supported.</span></span>|
|<span data-ttu-id="7af1e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7af1e-117">Application</span></span>|<span data-ttu-id="7af1e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7af1e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7af1e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7af1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7af1e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7af1e-120">Request headers</span></span>
|<span data-ttu-id="7af1e-121">标头</span><span class="sxs-lookup"><span data-stu-id="7af1e-121">Header</span></span>|<span data-ttu-id="7af1e-122">值</span><span class="sxs-lookup"><span data-stu-id="7af1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7af1e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7af1e-123">Authorization</span></span>|<span data-ttu-id="7af1e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7af1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7af1e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7af1e-125">Accept</span></span>|<span data-ttu-id="7af1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7af1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7af1e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7af1e-127">Request body</span></span>
<span data-ttu-id="7af1e-128">在请求正文中，提供[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7af1e-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="7af1e-129">下表显示时创建[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7af1e-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="7af1e-130">属性</span><span class="sxs-lookup"><span data-stu-id="7af1e-130">Property</span></span>|<span data-ttu-id="7af1e-131">类型</span><span class="sxs-lookup"><span data-stu-id="7af1e-131">Type</span></span>|<span data-ttu-id="7af1e-132">说明</span><span class="sxs-lookup"><span data-stu-id="7af1e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7af1e-133">id</span><span class="sxs-lookup"><span data-stu-id="7af1e-133">id</span></span>|<span data-ttu-id="7af1e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7af1e-134">String</span></span>|<span data-ttu-id="7af1e-135">Office 客户端配置策略的 id。</span><span class="sxs-lookup"><span data-stu-id="7af1e-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="7af1e-136">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="7af1e-137">userPreferencePayload</span></span>|<span data-ttu-id="7af1e-138">Stream</span><span class="sxs-lookup"><span data-stu-id="7af1e-138">Stream</span></span>|<span data-ttu-id="7af1e-139">首选项设置为 JSON 字符串以二进制格式，用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="7af1e-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="7af1e-140">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="7af1e-141">policyPayload</span></span>|<span data-ttu-id="7af1e-142">Stream</span><span class="sxs-lookup"><span data-stu-id="7af1e-142">Stream</span></span>|<span data-ttu-id="7af1e-143">策略设置 JSON 字符串以二进制格式，不能由用户更改这些值。</span><span class="sxs-lookup"><span data-stu-id="7af1e-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="7af1e-144">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-145">说明</span><span class="sxs-lookup"><span data-stu-id="7af1e-145">description</span></span>|<span data-ttu-id="7af1e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="7af1e-146">String</span></span>|<span data-ttu-id="7af1e-147">管理员提供的 office 客户端的说明配置策略。</span><span class="sxs-lookup"><span data-stu-id="7af1e-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="7af1e-148">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-149">displayName</span><span class="sxs-lookup"><span data-stu-id="7af1e-149">displayName</span></span>|<span data-ttu-id="7af1e-150">字符串</span><span class="sxs-lookup"><span data-stu-id="7af1e-150">String</span></span>|<span data-ttu-id="7af1e-151">管理员提供的 office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="7af1e-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="7af1e-152">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-153">assignments</span><span class="sxs-lookup"><span data-stu-id="7af1e-153">assignments</span></span>|<span data-ttu-id="7af1e-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="7af1e-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7af1e-155">策略的组分配列表正在</span><span class="sxs-lookup"><span data-stu-id="7af1e-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="7af1e-156">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-157">priority</span><span class="sxs-lookup"><span data-stu-id="7af1e-157">priority</span></span>|<span data-ttu-id="7af1e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7af1e-158">Int32</span></span>|<span data-ttu-id="7af1e-159">优先级值应为每个策略下租户的唯一值并将用于指定在冲突解决，较低值意味着很高的优先级。</span><span class="sxs-lookup"><span data-stu-id="7af1e-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="7af1e-160">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7af1e-161">lastModifiedDateTime</span></span>|<span data-ttu-id="7af1e-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="7af1e-162">DateTime</span></span>|<span data-ttu-id="7af1e-163">上次修改日期时间戳的策略。</span><span class="sxs-lookup"><span data-stu-id="7af1e-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="7af1e-164">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="7af1e-165">userCheckinSummary</span></span>|[<span data-ttu-id="7af1e-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="7af1e-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="7af1e-167">用户签入的摘要策略。</span><span class="sxs-lookup"><span data-stu-id="7af1e-167">User check-in summary for the policy.</span></span> <span data-ttu-id="7af1e-168">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7af1e-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="7af1e-169">checkinStatuses</span></span>|<span data-ttu-id="7af1e-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="7af1e-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="7af1e-171">Office 客户端中签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="7af1e-171">List of office Client check-in status.</span></span> <span data-ttu-id="7af1e-172">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7af1e-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7af1e-173">响应</span><span class="sxs-lookup"><span data-stu-id="7af1e-173">Response</span></span>
<span data-ttu-id="7af1e-174">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7af1e-174">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7af1e-175">示例</span><span class="sxs-lookup"><span data-stu-id="7af1e-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="7af1e-176">请求</span><span class="sxs-lookup"><span data-stu-id="7af1e-176">Request</span></span>
<span data-ttu-id="7af1e-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7af1e-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7af1e-178">响应</span><span class="sxs-lookup"><span data-stu-id="7af1e-178">Response</span></span>
<span data-ttu-id="7af1e-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7af1e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



