---
title: 创建 windowsOfficeClientConfiguration
description: 使用目标组创建新的非安全策略。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dffd413ca369378f3e3eccdbd1d3452b4854a72d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328236"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="ca70a-103">创建 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca70a-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="ca70a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca70a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca70a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca70a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca70a-106">使用目标组创建新的非安全策略。</span><span class="sxs-lookup"><span data-stu-id="ca70a-106">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca70a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca70a-107">Prerequisites</span></span>
<span data-ttu-id="ca70a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca70a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca70a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca70a-110">Permission type</span></span>|<span data-ttu-id="ca70a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca70a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca70a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca70a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca70a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca70a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca70a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca70a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca70a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca70a-115">Not supported.</span></span>|
|<span data-ttu-id="ca70a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca70a-116">Application</span></span>|<span data-ttu-id="ca70a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca70a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca70a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca70a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca70a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca70a-119">Request headers</span></span>
|<span data-ttu-id="ca70a-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca70a-120">Header</span></span>|<span data-ttu-id="ca70a-121">值</span><span class="sxs-lookup"><span data-stu-id="ca70a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca70a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca70a-122">Authorization</span></span>|<span data-ttu-id="ca70a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca70a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca70a-124">接受</span><span class="sxs-lookup"><span data-stu-id="ca70a-124">Accept</span></span>|<span data-ttu-id="ca70a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca70a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca70a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca70a-126">Request body</span></span>
<span data-ttu-id="ca70a-127">在请求正文中, 提供[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca70a-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="ca70a-128">下表显示创建[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca70a-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="ca70a-129">属性</span><span class="sxs-lookup"><span data-stu-id="ca70a-129">Property</span></span>|<span data-ttu-id="ca70a-130">类型</span><span class="sxs-lookup"><span data-stu-id="ca70a-130">Type</span></span>|<span data-ttu-id="ca70a-131">说明</span><span class="sxs-lookup"><span data-stu-id="ca70a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca70a-132">id</span><span class="sxs-lookup"><span data-stu-id="ca70a-132">id</span></span>|<span data-ttu-id="ca70a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ca70a-133">String</span></span>|<span data-ttu-id="ca70a-134">Office 客户端配置策略的 Id。</span><span class="sxs-lookup"><span data-stu-id="ca70a-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="ca70a-135">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="ca70a-136">userPreferencePayload</span></span>|<span data-ttu-id="ca70a-137">流</span><span class="sxs-lookup"><span data-stu-id="ca70a-137">Stream</span></span>|<span data-ttu-id="ca70a-138">首选项设置 JSON string 二进制格式, 则用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="ca70a-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="ca70a-139">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="ca70a-140">policyPayload</span></span>|<span data-ttu-id="ca70a-141">流</span><span class="sxs-lookup"><span data-stu-id="ca70a-141">Stream</span></span>|<span data-ttu-id="ca70a-142">策略设置 JSON string 二进制格式, 用户不能更改这些值。</span><span class="sxs-lookup"><span data-stu-id="ca70a-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="ca70a-143">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-144">说明</span><span class="sxs-lookup"><span data-stu-id="ca70a-144">description</span></span>|<span data-ttu-id="ca70a-145">String</span><span class="sxs-lookup"><span data-stu-id="ca70a-145">String</span></span>|<span data-ttu-id="ca70a-146">管理员提供的 office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ca70a-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="ca70a-147">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ca70a-148">displayName</span></span>|<span data-ttu-id="ca70a-149">String</span><span class="sxs-lookup"><span data-stu-id="ca70a-149">String</span></span>|<span data-ttu-id="ca70a-150">管理员提供的 office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="ca70a-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="ca70a-151">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-152">assignments</span><span class="sxs-lookup"><span data-stu-id="ca70a-152">assignments</span></span>|<span data-ttu-id="ca70a-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca70a-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ca70a-154">策略的组分配列表。。</span><span class="sxs-lookup"><span data-stu-id="ca70a-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="ca70a-155">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-156">priority</span><span class="sxs-lookup"><span data-stu-id="ca70a-156">priority</span></span>|<span data-ttu-id="ca70a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ca70a-157">Int32</span></span>|<span data-ttu-id="ca70a-158">对于租户下的每个策略, 优先级值应为唯一值, 并将用于冲突解决, 较低值意味着优先级较高。</span><span class="sxs-lookup"><span data-stu-id="ca70a-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="ca70a-159">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca70a-160">lastModifiedDateTime</span></span>|<span data-ttu-id="ca70a-161">日期时间</span><span class="sxs-lookup"><span data-stu-id="ca70a-161">DateTime</span></span>|<span data-ttu-id="ca70a-162">策略的上次修改日期时间戳。</span><span class="sxs-lookup"><span data-stu-id="ca70a-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="ca70a-163">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-164">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ca70a-164">userCheckinSummary</span></span>|[<span data-ttu-id="ca70a-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ca70a-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="ca70a-166">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="ca70a-166">User check-in summary for the policy.</span></span> <span data-ttu-id="ca70a-167">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ca70a-168">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="ca70a-168">checkinStatuses</span></span>|<span data-ttu-id="ca70a-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca70a-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="ca70a-170">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="ca70a-170">List of office Client check-in status.</span></span> <span data-ttu-id="ca70a-171">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca70a-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ca70a-172">响应</span><span class="sxs-lookup"><span data-stu-id="ca70a-172">Response</span></span>
<span data-ttu-id="ca70a-173">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca70a-173">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca70a-174">示例</span><span class="sxs-lookup"><span data-stu-id="ca70a-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca70a-175">请求</span><span class="sxs-lookup"><span data-stu-id="ca70a-175">Request</span></span>
<span data-ttu-id="ca70a-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca70a-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1020

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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

### <a name="response"></a><span data-ttu-id="ca70a-177">响应</span><span class="sxs-lookup"><span data-stu-id="ca70a-177">Response</span></span>
<span data-ttu-id="ca70a-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca70a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
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






