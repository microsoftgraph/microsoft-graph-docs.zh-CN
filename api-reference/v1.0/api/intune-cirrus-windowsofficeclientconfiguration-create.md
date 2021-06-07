---
title: 创建 windowsOfficeClientConfiguration
description: 使用目标组创建新的非安全策略。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 159a99785a63e74f863c977a8c0bfe933f8ced75
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754344"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="7f612-103">创建 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f612-103">Create windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="7f612-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f612-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f612-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f612-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f612-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f612-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f612-107">使用目标组创建新的非安全策略。</span><span class="sxs-lookup"><span data-stu-id="7f612-107">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f612-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f612-108">Prerequisites</span></span>
<span data-ttu-id="7f612-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f612-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f612-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f612-111">Permission type</span></span>|<span data-ttu-id="7f612-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f612-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f612-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f612-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f612-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f612-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f612-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f612-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f612-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f612-116">Not supported.</span></span>|
|<span data-ttu-id="7f612-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f612-117">Application</span></span>|<span data-ttu-id="7f612-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f612-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f612-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f612-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f612-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f612-120">Request headers</span></span>
|<span data-ttu-id="7f612-121">标头</span><span class="sxs-lookup"><span data-stu-id="7f612-121">Header</span></span>|<span data-ttu-id="7f612-122">值</span><span class="sxs-lookup"><span data-stu-id="7f612-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f612-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f612-123">Authorization</span></span>|<span data-ttu-id="7f612-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f612-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f612-125">接受</span><span class="sxs-lookup"><span data-stu-id="7f612-125">Accept</span></span>|<span data-ttu-id="7f612-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f612-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f612-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f612-127">Request body</span></span>
<span data-ttu-id="7f612-128">在请求正文中，提供 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f612-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="7f612-129">下表显示创建 [windowsOfficeClientConfiguration 时所需的属性](../resources/intune-cirrus-windowsofficeclientconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7f612-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="7f612-130">属性</span><span class="sxs-lookup"><span data-stu-id="7f612-130">Property</span></span>|<span data-ttu-id="7f612-131">类型</span><span class="sxs-lookup"><span data-stu-id="7f612-131">Type</span></span>|<span data-ttu-id="7f612-132">说明</span><span class="sxs-lookup"><span data-stu-id="7f612-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f612-133">id</span><span class="sxs-lookup"><span data-stu-id="7f612-133">id</span></span>|<span data-ttu-id="7f612-134">String</span><span class="sxs-lookup"><span data-stu-id="7f612-134">String</span></span>|<span data-ttu-id="7f612-135">Office 客户端配置策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="7f612-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="7f612-136">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="7f612-137">userPreferencePayload</span></span>|<span data-ttu-id="7f612-138">Stream</span><span class="sxs-lookup"><span data-stu-id="7f612-138">Stream</span></span>|<span data-ttu-id="7f612-139">首选项设置 二进制格式的 JSON 字符串，用户可以替代这些值。</span><span class="sxs-lookup"><span data-stu-id="7f612-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="7f612-140">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="7f612-141">policyPayload</span></span>|<span data-ttu-id="7f612-142">Stream</span><span class="sxs-lookup"><span data-stu-id="7f612-142">Stream</span></span>|<span data-ttu-id="7f612-143">策略设置 二进制格式的 JSON 字符串，用户无法更改这些值。</span><span class="sxs-lookup"><span data-stu-id="7f612-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="7f612-144">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-145">description</span><span class="sxs-lookup"><span data-stu-id="7f612-145">description</span></span>|<span data-ttu-id="7f612-146">String</span><span class="sxs-lookup"><span data-stu-id="7f612-146">String</span></span>|<span data-ttu-id="7f612-147">管理员提供了 Office 客户端配置策略的说明。</span><span class="sxs-lookup"><span data-stu-id="7f612-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="7f612-148">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-149">displayName</span><span class="sxs-lookup"><span data-stu-id="7f612-149">displayName</span></span>|<span data-ttu-id="7f612-150">String</span><span class="sxs-lookup"><span data-stu-id="7f612-150">String</span></span>|<span data-ttu-id="7f612-151">管理员提供的 Office 客户端配置策略的名称。</span><span class="sxs-lookup"><span data-stu-id="7f612-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="7f612-152">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-153">assignments</span><span class="sxs-lookup"><span data-stu-id="7f612-153">assignments</span></span>|<span data-ttu-id="7f612-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f612-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7f612-155">策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="7f612-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="7f612-156">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-157">priority</span><span class="sxs-lookup"><span data-stu-id="7f612-157">priority</span></span>|<span data-ttu-id="7f612-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7f612-158">Int32</span></span>|<span data-ttu-id="7f612-159">优先级值应为租户下每个策略的唯一值，并且将用于冲突解决，较低的值表示优先级较高。</span><span class="sxs-lookup"><span data-stu-id="7f612-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="7f612-160">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f612-161">lastModifiedDateTime</span></span>|<span data-ttu-id="7f612-162">日期时间</span><span class="sxs-lookup"><span data-stu-id="7f612-162">DateTime</span></span>|<span data-ttu-id="7f612-163">策略的上次修改日期/时间戳。</span><span class="sxs-lookup"><span data-stu-id="7f612-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="7f612-164">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="7f612-165">userCheckinSummary</span></span>|[<span data-ttu-id="7f612-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="7f612-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="7f612-167">策略的用户签入摘要。</span><span class="sxs-lookup"><span data-stu-id="7f612-167">User check-in summary for the policy.</span></span> <span data-ttu-id="7f612-168">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7f612-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="7f612-169">checkinStatuses</span></span>|<span data-ttu-id="7f612-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f612-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="7f612-171">Office 客户端签入状态列表。</span><span class="sxs-lookup"><span data-stu-id="7f612-171">List of office Client check-in status.</span></span> <span data-ttu-id="7f612-172">继承自 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f612-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7f612-173">响应</span><span class="sxs-lookup"><span data-stu-id="7f612-173">Response</span></span>
<span data-ttu-id="7f612-174">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f612-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f612-175">示例</span><span class="sxs-lookup"><span data-stu-id="7f612-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f612-176">请求</span><span class="sxs-lookup"><span data-stu-id="7f612-176">Request</span></span>
<span data-ttu-id="7f612-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f612-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f612-178">响应</span><span class="sxs-lookup"><span data-stu-id="7f612-178">Response</span></span>
<span data-ttu-id="7f612-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f612-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




