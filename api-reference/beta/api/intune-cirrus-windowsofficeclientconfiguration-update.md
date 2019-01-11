---
title: 更新 windowsOfficeClientConfiguration
description: 修补程序特定的非安全策略负载。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e13228c6fc467fa49b740c02b4b7068efb1ec42e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863873"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="be58e-103">更新 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="be58e-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="be58e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="be58e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be58e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be58e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be58e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="be58e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be58e-107">修补程序特定的非安全策略负载。</span><span class="sxs-lookup"><span data-stu-id="be58e-107">Patch a specific non-security policy payload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be58e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="be58e-108">Prerequisites</span></span>
<span data-ttu-id="be58e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="be58e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be58e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="be58e-111">Permission type</span></span>|<span data-ttu-id="be58e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be58e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be58e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be58e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be58e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be58e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be58e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be58e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be58e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be58e-116">Not supported.</span></span>|
|<span data-ttu-id="be58e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="be58e-117">Application</span></span>|<span data-ttu-id="be58e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="be58e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be58e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be58e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="be58e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="be58e-120">Request headers</span></span>
|<span data-ttu-id="be58e-121">标头</span><span class="sxs-lookup"><span data-stu-id="be58e-121">Header</span></span>|<span data-ttu-id="be58e-122">值</span><span class="sxs-lookup"><span data-stu-id="be58e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be58e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be58e-123">Authorization</span></span>|<span data-ttu-id="be58e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be58e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be58e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be58e-125">Accept</span></span>|<span data-ttu-id="be58e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be58e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be58e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="be58e-127">Request body</span></span>
<span data-ttu-id="be58e-128">在请求正文中，提供[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be58e-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="be58e-129">下表显示时创建[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be58e-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="be58e-130">属性</span><span class="sxs-lookup"><span data-stu-id="be58e-130">Property</span></span>|<span data-ttu-id="be58e-131">类型</span><span class="sxs-lookup"><span data-stu-id="be58e-131">Type</span></span>|<span data-ttu-id="be58e-132">说明</span><span class="sxs-lookup"><span data-stu-id="be58e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be58e-133">id</span><span class="sxs-lookup"><span data-stu-id="be58e-133">id</span></span>|<span data-ttu-id="be58e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="be58e-134">String</span></span>|<span data-ttu-id="be58e-135">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="be58e-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="be58e-136">userPreferencePayload</span></span>|<span data-ttu-id="be58e-137">Stream</span><span class="sxs-lookup"><span data-stu-id="be58e-137">Stream</span></span>|<span data-ttu-id="be58e-138">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="be58e-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="be58e-139">policyPayload</span></span>|<span data-ttu-id="be58e-140">Stream</span><span class="sxs-lookup"><span data-stu-id="be58e-140">Stream</span></span>|<span data-ttu-id="be58e-141">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="be58e-142">说明</span><span class="sxs-lookup"><span data-stu-id="be58e-142">description</span></span>|<span data-ttu-id="be58e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="be58e-143">String</span></span>|<span data-ttu-id="be58e-144">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="be58e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="be58e-145">displayName</span></span>|<span data-ttu-id="be58e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="be58e-146">String</span></span>|<span data-ttu-id="be58e-147">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="be58e-148">priority</span><span class="sxs-lookup"><span data-stu-id="be58e-148">priority</span></span>|<span data-ttu-id="be58e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="be58e-149">Int32</span></span>|<span data-ttu-id="be58e-150">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="be58e-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="be58e-151">userCheckinSummary</span></span>|[<span data-ttu-id="be58e-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="be58e-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="be58e-153">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="be58e-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="be58e-154">checkinStatuses</span></span>|<span data-ttu-id="be58e-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="be58e-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="be58e-156">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="be58e-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="be58e-157">响应</span><span class="sxs-lookup"><span data-stu-id="be58e-157">Response</span></span>
<span data-ttu-id="be58e-158">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="be58e-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be58e-159">示例</span><span class="sxs-lookup"><span data-stu-id="be58e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="be58e-160">请求</span><span class="sxs-lookup"><span data-stu-id="be58e-160">Request</span></span>
<span data-ttu-id="be58e-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be58e-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be58e-162">响应</span><span class="sxs-lookup"><span data-stu-id="be58e-162">Response</span></span>
<span data-ttu-id="be58e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be58e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



