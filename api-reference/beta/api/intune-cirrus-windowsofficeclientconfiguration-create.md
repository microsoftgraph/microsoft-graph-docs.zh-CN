---
title: 创建 windowsOfficeClientConfiguration
description: 与目标组中创建新的非安全策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a915447ad22438d021bb4577fc856bbe89db1fdc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394374"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="421ba-103">创建 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="421ba-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="421ba-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="421ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="421ba-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="421ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="421ba-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="421ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421ba-107">与目标组中创建新的非安全策略。</span><span class="sxs-lookup"><span data-stu-id="421ba-107">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="421ba-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="421ba-108">Prerequisites</span></span>
<span data-ttu-id="421ba-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="421ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421ba-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="421ba-111">Permission type</span></span>|<span data-ttu-id="421ba-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="421ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="421ba-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="421ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="421ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="421ba-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="421ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="421ba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="421ba-116">Not supported.</span></span>|
|<span data-ttu-id="421ba-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="421ba-117">Application</span></span>|<span data-ttu-id="421ba-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="421ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="421ba-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="421ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="421ba-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="421ba-120">Request headers</span></span>
|<span data-ttu-id="421ba-121">标头</span><span class="sxs-lookup"><span data-stu-id="421ba-121">Header</span></span>|<span data-ttu-id="421ba-122">值</span><span class="sxs-lookup"><span data-stu-id="421ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="421ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="421ba-123">Authorization</span></span>|<span data-ttu-id="421ba-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="421ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="421ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="421ba-125">Accept</span></span>|<span data-ttu-id="421ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="421ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="421ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="421ba-127">Request body</span></span>
<span data-ttu-id="421ba-128">在请求正文中，提供[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="421ba-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="421ba-129">下表显示时创建[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="421ba-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="421ba-130">属性</span><span class="sxs-lookup"><span data-stu-id="421ba-130">Property</span></span>|<span data-ttu-id="421ba-131">类型</span><span class="sxs-lookup"><span data-stu-id="421ba-131">Type</span></span>|<span data-ttu-id="421ba-132">说明</span><span class="sxs-lookup"><span data-stu-id="421ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421ba-133">id</span><span class="sxs-lookup"><span data-stu-id="421ba-133">id</span></span>|<span data-ttu-id="421ba-134">String</span><span class="sxs-lookup"><span data-stu-id="421ba-134">String</span></span>|<span data-ttu-id="421ba-135">Office 客户端配置策略的 id。</span><span class="sxs-lookup"><span data-stu-id="421ba-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="421ba-136">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="421ba-137">userPreferencePayload</span></span>|<span data-ttu-id="421ba-138">Stream</span><span class="sxs-lookup"><span data-stu-id="421ba-138">Stream</span></span>|<span data-ttu-id="421ba-139">首选项设置为 JSON 字符串以二进制格式，用户可以重写这些值。</span><span class="sxs-lookup"><span data-stu-id="421ba-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="421ba-140">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="421ba-141">policyPayload</span></span>|<span data-ttu-id="421ba-142">Stream</span><span class="sxs-lookup"><span data-stu-id="421ba-142">Stream</span></span>|<span data-ttu-id="421ba-143">策略设置 JSON 字符串以二进制格式，不能由用户更改这些值。</span><span class="sxs-lookup"><span data-stu-id="421ba-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="421ba-144">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-145">说明</span><span class="sxs-lookup"><span data-stu-id="421ba-145">description</span></span>|<span data-ttu-id="421ba-146">String</span><span class="sxs-lookup"><span data-stu-id="421ba-146">String</span></span>|<span data-ttu-id="421ba-147">管理员提供的 office 客户端的说明配置策略。</span><span class="sxs-lookup"><span data-stu-id="421ba-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="421ba-148">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-149">displayName</span><span class="sxs-lookup"><span data-stu-id="421ba-149">displayName</span></span>|<span data-ttu-id="421ba-150">String</span><span class="sxs-lookup"><span data-stu-id="421ba-150">String</span></span>|<span data-ttu-id="421ba-151">管理员提供的 office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="421ba-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="421ba-152">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-153">assignments</span><span class="sxs-lookup"><span data-stu-id="421ba-153">assignments</span></span>|<span data-ttu-id="421ba-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="421ba-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="421ba-155">策略的组分配列表正在</span><span class="sxs-lookup"><span data-stu-id="421ba-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="421ba-156">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-157">priority</span><span class="sxs-lookup"><span data-stu-id="421ba-157">priority</span></span>|<span data-ttu-id="421ba-158">Int32</span><span class="sxs-lookup"><span data-stu-id="421ba-158">Int32</span></span>|<span data-ttu-id="421ba-159">优先级值应为每个策略下租户的唯一值并将用于指定在冲突解决，较低值意味着很高的优先级。</span><span class="sxs-lookup"><span data-stu-id="421ba-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="421ba-160">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="421ba-161">lastModifiedDateTime</span></span>|<span data-ttu-id="421ba-162">日期/时间</span><span class="sxs-lookup"><span data-stu-id="421ba-162">DateTime</span></span>|<span data-ttu-id="421ba-163">上次修改日期时间戳的策略。</span><span class="sxs-lookup"><span data-stu-id="421ba-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="421ba-164">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="421ba-165">userCheckinSummary</span></span>|[<span data-ttu-id="421ba-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="421ba-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="421ba-167">用户签入的摘要策略。</span><span class="sxs-lookup"><span data-stu-id="421ba-167">User check-in summary for the policy.</span></span> <span data-ttu-id="421ba-168">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="421ba-169">checkinStatuses</span></span>|<span data-ttu-id="421ba-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="421ba-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="421ba-171">Office 客户端中签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="421ba-171">List of office Client check-in status.</span></span> <span data-ttu-id="421ba-172">继承自[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="421ba-173">响应</span><span class="sxs-lookup"><span data-stu-id="421ba-173">Response</span></span>
<span data-ttu-id="421ba-174">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="421ba-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="421ba-175">示例</span><span class="sxs-lookup"><span data-stu-id="421ba-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="421ba-176">请求</span><span class="sxs-lookup"><span data-stu-id="421ba-176">Request</span></span>
<span data-ttu-id="421ba-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="421ba-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="421ba-178">响应</span><span class="sxs-lookup"><span data-stu-id="421ba-178">Response</span></span>
<span data-ttu-id="421ba-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="421ba-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



