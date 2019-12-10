---
title: 更新 windowsOfficeClientConfiguration
description: 修补特定的非安全策略有效负载。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dec76e1e8edd7eae2ff001f2e5cf76ffd57029e4
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39930399"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="ae2c2-103">更新 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae2c2-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="ae2c2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae2c2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae2c2-106">修补特定的非安全策略有效负载。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-106">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae2c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ae2c2-107">Prerequisites</span></span>
<span data-ttu-id="ae2c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae2c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae2c2-110">Permission type</span></span>|<span data-ttu-id="ae2c2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ae2c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae2c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae2c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae2c2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae2c2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae2c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae2c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae2c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-115">Not supported.</span></span>|
|<span data-ttu-id="ae2c2-116">Application</span><span class="sxs-lookup"><span data-stu-id="ae2c2-116">Application</span></span>|<span data-ttu-id="ae2c2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae2c2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae2c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae2c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="ae2c2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae2c2-119">Request headers</span></span>
|<span data-ttu-id="ae2c2-120">标头</span><span class="sxs-lookup"><span data-stu-id="ae2c2-120">Header</span></span>|<span data-ttu-id="ae2c2-121">值</span><span class="sxs-lookup"><span data-stu-id="ae2c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae2c2-122">授权</span><span class="sxs-lookup"><span data-stu-id="ae2c2-122">Authorization</span></span>|<span data-ttu-id="ae2c2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae2c2-124">接受</span><span class="sxs-lookup"><span data-stu-id="ae2c2-124">Accept</span></span>|<span data-ttu-id="ae2c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae2c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae2c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae2c2-126">Request body</span></span>
<span data-ttu-id="ae2c2-127">在请求正文中，提供[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="ae2c2-128">下表显示创建[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="ae2c2-129">属性</span><span class="sxs-lookup"><span data-stu-id="ae2c2-129">Property</span></span>|<span data-ttu-id="ae2c2-130">类型</span><span class="sxs-lookup"><span data-stu-id="ae2c2-130">Type</span></span>|<span data-ttu-id="ae2c2-131">说明</span><span class="sxs-lookup"><span data-stu-id="ae2c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae2c2-132">id</span><span class="sxs-lookup"><span data-stu-id="ae2c2-132">id</span></span>|<span data-ttu-id="ae2c2-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ae2c2-133">String</span></span>|<span data-ttu-id="ae2c2-134">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-134">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ae2c2-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="ae2c2-135">userPreferencePayload</span></span>|<span data-ttu-id="ae2c2-136">Stream</span><span class="sxs-lookup"><span data-stu-id="ae2c2-136">Stream</span></span>|<span data-ttu-id="ae2c2-137">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-137">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ae2c2-138">policyPayload</span><span class="sxs-lookup"><span data-stu-id="ae2c2-138">policyPayload</span></span>|<span data-ttu-id="ae2c2-139">Stream</span><span class="sxs-lookup"><span data-stu-id="ae2c2-139">Stream</span></span>|<span data-ttu-id="ae2c2-140">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-140">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ae2c2-141">说明</span><span class="sxs-lookup"><span data-stu-id="ae2c2-141">description</span></span>|<span data-ttu-id="ae2c2-142">String</span><span class="sxs-lookup"><span data-stu-id="ae2c2-142">String</span></span>|<span data-ttu-id="ae2c2-143">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-143">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ae2c2-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ae2c2-144">displayName</span></span>|<span data-ttu-id="ae2c2-145">String</span><span class="sxs-lookup"><span data-stu-id="ae2c2-145">String</span></span>|<span data-ttu-id="ae2c2-146">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-146">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ae2c2-147">priority</span><span class="sxs-lookup"><span data-stu-id="ae2c2-147">priority</span></span>|<span data-ttu-id="ae2c2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ae2c2-148">Int32</span></span>|<span data-ttu-id="ae2c2-149">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-149">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ae2c2-150">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ae2c2-150">userCheckinSummary</span></span>|[<span data-ttu-id="ae2c2-151">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ae2c2-151">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="ae2c2-152">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-152">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ae2c2-153">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="ae2c2-153">checkinStatuses</span></span>|<span data-ttu-id="ae2c2-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="ae2c2-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="ae2c2-155">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="ae2c2-155">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ae2c2-156">响应</span><span class="sxs-lookup"><span data-stu-id="ae2c2-156">Response</span></span>
<span data-ttu-id="ae2c2-157">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-157">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae2c2-158">示例</span><span class="sxs-lookup"><span data-stu-id="ae2c2-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae2c2-159">请求</span><span class="sxs-lookup"><span data-stu-id="ae2c2-159">Request</span></span>
<span data-ttu-id="ae2c2-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ae2c2-161">响应</span><span class="sxs-lookup"><span data-stu-id="ae2c2-161">Response</span></span>
<span data-ttu-id="ae2c2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae2c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





