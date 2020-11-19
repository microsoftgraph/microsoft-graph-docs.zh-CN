---
title: 更新 windowsOfficeClientConfiguration
description: 修补特定的非安全策略有效负载。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f62b8ebb03efcab5975fabe8d1c5606bd176af5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49244239"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="a4d71-103">更新 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4d71-103">Update windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="a4d71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4d71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4d71-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4d71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4d71-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4d71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4d71-107">修补特定的非安全策略有效负载。</span><span class="sxs-lookup"><span data-stu-id="a4d71-107">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4d71-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4d71-108">Prerequisites</span></span>
<span data-ttu-id="a4d71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4d71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4d71-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4d71-111">Permission type</span></span>|<span data-ttu-id="a4d71-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4d71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4d71-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4d71-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4d71-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4d71-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4d71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4d71-116">Not supported.</span></span>|
|<span data-ttu-id="a4d71-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4d71-117">Application</span></span>|<span data-ttu-id="a4d71-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4d71-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4d71-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4d71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="a4d71-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4d71-120">Request headers</span></span>
|<span data-ttu-id="a4d71-121">标头</span><span class="sxs-lookup"><span data-stu-id="a4d71-121">Header</span></span>|<span data-ttu-id="a4d71-122">值</span><span class="sxs-lookup"><span data-stu-id="a4d71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4d71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4d71-123">Authorization</span></span>|<span data-ttu-id="a4d71-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4d71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4d71-125">接受</span><span class="sxs-lookup"><span data-stu-id="a4d71-125">Accept</span></span>|<span data-ttu-id="a4d71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4d71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4d71-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4d71-127">Request body</span></span>
<span data-ttu-id="a4d71-128">在请求正文中，提供 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4d71-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="a4d71-129">下表显示创建 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4d71-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="a4d71-130">属性</span><span class="sxs-lookup"><span data-stu-id="a4d71-130">Property</span></span>|<span data-ttu-id="a4d71-131">类型</span><span class="sxs-lookup"><span data-stu-id="a4d71-131">Type</span></span>|<span data-ttu-id="a4d71-132">说明</span><span class="sxs-lookup"><span data-stu-id="a4d71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4d71-133">id</span><span class="sxs-lookup"><span data-stu-id="a4d71-133">id</span></span>|<span data-ttu-id="a4d71-134">String</span><span class="sxs-lookup"><span data-stu-id="a4d71-134">String</span></span>|<span data-ttu-id="a4d71-135">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="a4d71-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="a4d71-136">userPreferencePayload</span></span>|<span data-ttu-id="a4d71-137">Stream</span><span class="sxs-lookup"><span data-stu-id="a4d71-137">Stream</span></span>|<span data-ttu-id="a4d71-138">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="a4d71-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="a4d71-139">policyPayload</span></span>|<span data-ttu-id="a4d71-140">Stream</span><span class="sxs-lookup"><span data-stu-id="a4d71-140">Stream</span></span>|<span data-ttu-id="a4d71-141">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="a4d71-142">description</span><span class="sxs-lookup"><span data-stu-id="a4d71-142">description</span></span>|<span data-ttu-id="a4d71-143">String</span><span class="sxs-lookup"><span data-stu-id="a4d71-143">String</span></span>|<span data-ttu-id="a4d71-144">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="a4d71-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a4d71-145">displayName</span></span>|<span data-ttu-id="a4d71-146">String</span><span class="sxs-lookup"><span data-stu-id="a4d71-146">String</span></span>|<span data-ttu-id="a4d71-147">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="a4d71-148">priority</span><span class="sxs-lookup"><span data-stu-id="a4d71-148">priority</span></span>|<span data-ttu-id="a4d71-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a4d71-149">Int32</span></span>|<span data-ttu-id="a4d71-150">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="a4d71-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="a4d71-151">userCheckinSummary</span></span>|[<span data-ttu-id="a4d71-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="a4d71-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="a4d71-153">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="a4d71-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="a4d71-154">checkinStatuses</span></span>|<span data-ttu-id="a4d71-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a4d71-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="a4d71-156">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="a4d71-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a4d71-157">响应</span><span class="sxs-lookup"><span data-stu-id="a4d71-157">Response</span></span>
<span data-ttu-id="a4d71-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4d71-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4d71-159">示例</span><span class="sxs-lookup"><span data-stu-id="a4d71-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4d71-160">请求</span><span class="sxs-lookup"><span data-stu-id="a4d71-160">Request</span></span>
<span data-ttu-id="a4d71-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4d71-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4d71-162">响应</span><span class="sxs-lookup"><span data-stu-id="a4d71-162">Response</span></span>
<span data-ttu-id="a4d71-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4d71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




