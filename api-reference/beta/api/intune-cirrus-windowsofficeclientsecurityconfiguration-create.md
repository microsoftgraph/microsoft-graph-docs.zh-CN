---
title: 创建 windowsOfficeClientSecurityConfiguration
description: 创建新的 windowsOfficeClientSecurityConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 011212ddfe1790ebfb0c6191a41e4ba670555171
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324715"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="0865d-103">创建 windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="0865d-103">Create windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="0865d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0865d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0865d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0865d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0865d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0865d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0865d-107">创建新的[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0865d-107">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0865d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0865d-108">Prerequisites</span></span>
<span data-ttu-id="0865d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0865d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0865d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0865d-111">Permission type</span></span>|<span data-ttu-id="0865d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0865d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0865d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0865d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0865d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0865d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0865d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0865d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0865d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0865d-116">Not supported.</span></span>|
|<span data-ttu-id="0865d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0865d-117">Application</span></span>|<span data-ttu-id="0865d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0865d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0865d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0865d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0865d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0865d-120">Request headers</span></span>
|<span data-ttu-id="0865d-121">标头</span><span class="sxs-lookup"><span data-stu-id="0865d-121">Header</span></span>|<span data-ttu-id="0865d-122">值</span><span class="sxs-lookup"><span data-stu-id="0865d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0865d-123">授权</span><span class="sxs-lookup"><span data-stu-id="0865d-123">Authorization</span></span>|<span data-ttu-id="0865d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0865d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0865d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0865d-125">Accept</span></span>|<span data-ttu-id="0865d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0865d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0865d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0865d-127">Request body</span></span>
<span data-ttu-id="0865d-128">在请求正文中，提供[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0865d-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="0865d-129">下表显示时创建[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0865d-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="0865d-130">属性</span><span class="sxs-lookup"><span data-stu-id="0865d-130">Property</span></span>|<span data-ttu-id="0865d-131">类型</span><span class="sxs-lookup"><span data-stu-id="0865d-131">Type</span></span>|<span data-ttu-id="0865d-132">说明</span><span class="sxs-lookup"><span data-stu-id="0865d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0865d-133">id</span><span class="sxs-lookup"><span data-stu-id="0865d-133">id</span></span>|<span data-ttu-id="0865d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="0865d-134">String</span></span>|<span data-ttu-id="0865d-135">Office 客户端配置策略的 id。</span><span class="sxs-lookup"><span data-stu-id="0865d-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="0865d-136">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="0865d-137">userPreferencePayload</span></span>|<span data-ttu-id="0865d-138">Stream</span><span class="sxs-lookup"><span data-stu-id="0865d-138">Stream</span></span>|<span data-ttu-id="0865d-139">首选项设置为 JSON 字符串以二进制格式，用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="0865d-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="0865d-140">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="0865d-141">policyPayload</span></span>|<span data-ttu-id="0865d-142">Stream</span><span class="sxs-lookup"><span data-stu-id="0865d-142">Stream</span></span>|<span data-ttu-id="0865d-143">策略设置 JSON 字符串以二进制格式，不能由用户更改这些值。</span><span class="sxs-lookup"><span data-stu-id="0865d-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="0865d-144">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-145">说明</span><span class="sxs-lookup"><span data-stu-id="0865d-145">description</span></span>|<span data-ttu-id="0865d-146">字符串</span><span class="sxs-lookup"><span data-stu-id="0865d-146">String</span></span>|<span data-ttu-id="0865d-147">管理员提供的 office 客户端的说明配置策略。</span><span class="sxs-lookup"><span data-stu-id="0865d-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="0865d-148">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-149">displayName</span><span class="sxs-lookup"><span data-stu-id="0865d-149">displayName</span></span>|<span data-ttu-id="0865d-150">字符串</span><span class="sxs-lookup"><span data-stu-id="0865d-150">String</span></span>|<span data-ttu-id="0865d-151">管理员提供的 office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="0865d-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="0865d-152">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-153">assignments</span><span class="sxs-lookup"><span data-stu-id="0865d-153">assignments</span></span>|<span data-ttu-id="0865d-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0865d-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0865d-155">策略的组分配列表正在</span><span class="sxs-lookup"><span data-stu-id="0865d-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="0865d-156">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-157">priority</span><span class="sxs-lookup"><span data-stu-id="0865d-157">priority</span></span>|<span data-ttu-id="0865d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0865d-158">Int32</span></span>|<span data-ttu-id="0865d-159">优先级值应为每个策略下租户的唯一值并将用于指定在冲突解决，较低值意味着很高的优先级。</span><span class="sxs-lookup"><span data-stu-id="0865d-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="0865d-160">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0865d-161">lastModifiedDateTime</span></span>|<span data-ttu-id="0865d-162">日期时间</span><span class="sxs-lookup"><span data-stu-id="0865d-162">DateTime</span></span>|<span data-ttu-id="0865d-163">上次修改日期时间戳的策略。</span><span class="sxs-lookup"><span data-stu-id="0865d-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="0865d-164">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0865d-165">userCheckinSummary</span></span>|[<span data-ttu-id="0865d-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0865d-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="0865d-167">用户签入的摘要策略。</span><span class="sxs-lookup"><span data-stu-id="0865d-167">User check-in summary for the policy.</span></span> <span data-ttu-id="0865d-168">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0865d-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="0865d-169">checkinStatuses</span></span>|<span data-ttu-id="0865d-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="0865d-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="0865d-171">Office 客户端中签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="0865d-171">List of office Client check-in status.</span></span> <span data-ttu-id="0865d-172">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0865d-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="0865d-173">响应</span><span class="sxs-lookup"><span data-stu-id="0865d-173">Response</span></span>
<span data-ttu-id="0865d-174">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0865d-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0865d-175">示例</span><span class="sxs-lookup"><span data-stu-id="0865d-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="0865d-176">请求</span><span class="sxs-lookup"><span data-stu-id="0865d-176">Request</span></span>
<span data-ttu-id="0865d-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0865d-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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

### <a name="response"></a><span data-ttu-id="0865d-178">响应</span><span class="sxs-lookup"><span data-stu-id="0865d-178">Response</span></span>
<span data-ttu-id="0865d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0865d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



