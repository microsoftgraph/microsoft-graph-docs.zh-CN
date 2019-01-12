---
title: 更新 windowsOfficeClientConfiguration
description: 修补程序特定的非安全策略负载。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76179dadc4620617487c66b719626778fa4e4f26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983504"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="38bdd-103">更新 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="38bdd-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="38bdd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38bdd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38bdd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38bdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38bdd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="38bdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38bdd-107">修补程序特定的非安全策略负载。</span><span class="sxs-lookup"><span data-stu-id="38bdd-107">Patch a specific non-security policy payload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38bdd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="38bdd-108">Prerequisites</span></span>
<span data-ttu-id="38bdd-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="38bdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38bdd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38bdd-111">Permission type</span></span>|<span data-ttu-id="38bdd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38bdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38bdd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38bdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38bdd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38bdd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38bdd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38bdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38bdd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38bdd-116">Not supported.</span></span>|
|<span data-ttu-id="38bdd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="38bdd-117">Application</span></span>|<span data-ttu-id="38bdd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="38bdd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38bdd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38bdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="38bdd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="38bdd-120">Request headers</span></span>
|<span data-ttu-id="38bdd-121">标头</span><span class="sxs-lookup"><span data-stu-id="38bdd-121">Header</span></span>|<span data-ttu-id="38bdd-122">值</span><span class="sxs-lookup"><span data-stu-id="38bdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38bdd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38bdd-123">Authorization</span></span>|<span data-ttu-id="38bdd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38bdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38bdd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38bdd-125">Accept</span></span>|<span data-ttu-id="38bdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38bdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38bdd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38bdd-127">Request body</span></span>
<span data-ttu-id="38bdd-128">在请求正文中，提供[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38bdd-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="38bdd-129">下表显示时创建[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38bdd-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="38bdd-130">属性</span><span class="sxs-lookup"><span data-stu-id="38bdd-130">Property</span></span>|<span data-ttu-id="38bdd-131">类型</span><span class="sxs-lookup"><span data-stu-id="38bdd-131">Type</span></span>|<span data-ttu-id="38bdd-132">说明</span><span class="sxs-lookup"><span data-stu-id="38bdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38bdd-133">id</span><span class="sxs-lookup"><span data-stu-id="38bdd-133">id</span></span>|<span data-ttu-id="38bdd-134">字符串</span><span class="sxs-lookup"><span data-stu-id="38bdd-134">String</span></span>|<span data-ttu-id="38bdd-135">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="38bdd-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="38bdd-136">userPreferencePayload</span></span>|<span data-ttu-id="38bdd-137">Stream</span><span class="sxs-lookup"><span data-stu-id="38bdd-137">Stream</span></span>|<span data-ttu-id="38bdd-138">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="38bdd-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="38bdd-139">policyPayload</span></span>|<span data-ttu-id="38bdd-140">Stream</span><span class="sxs-lookup"><span data-stu-id="38bdd-140">Stream</span></span>|<span data-ttu-id="38bdd-141">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="38bdd-142">说明</span><span class="sxs-lookup"><span data-stu-id="38bdd-142">description</span></span>|<span data-ttu-id="38bdd-143">字符串</span><span class="sxs-lookup"><span data-stu-id="38bdd-143">String</span></span>|<span data-ttu-id="38bdd-144">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="38bdd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="38bdd-145">displayName</span></span>|<span data-ttu-id="38bdd-146">字符串</span><span class="sxs-lookup"><span data-stu-id="38bdd-146">String</span></span>|<span data-ttu-id="38bdd-147">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="38bdd-148">priority</span><span class="sxs-lookup"><span data-stu-id="38bdd-148">priority</span></span>|<span data-ttu-id="38bdd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="38bdd-149">Int32</span></span>|<span data-ttu-id="38bdd-150">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="38bdd-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="38bdd-151">userCheckinSummary</span></span>|[<span data-ttu-id="38bdd-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="38bdd-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="38bdd-153">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="38bdd-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="38bdd-154">checkinStatuses</span></span>|<span data-ttu-id="38bdd-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="38bdd-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="38bdd-156">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)记录继承</span><span class="sxs-lookup"><span data-stu-id="38bdd-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="38bdd-157">响应</span><span class="sxs-lookup"><span data-stu-id="38bdd-157">Response</span></span>
<span data-ttu-id="38bdd-158">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38bdd-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38bdd-159">示例</span><span class="sxs-lookup"><span data-stu-id="38bdd-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="38bdd-160">请求</span><span class="sxs-lookup"><span data-stu-id="38bdd-160">Request</span></span>
<span data-ttu-id="38bdd-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38bdd-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38bdd-162">响应</span><span class="sxs-lookup"><span data-stu-id="38bdd-162">Response</span></span>
<span data-ttu-id="38bdd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38bdd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



