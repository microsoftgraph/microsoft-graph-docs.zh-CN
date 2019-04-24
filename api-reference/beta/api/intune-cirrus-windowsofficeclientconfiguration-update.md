---
title: 更新 windowsOfficeClientConfiguration
description: 修补特定的非安全策略有效负载。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d116d846b6540ea2b9e2a91f54a5abdfa81e2409
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483290"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="de015-103">更新 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="de015-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="de015-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de015-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de015-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de015-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de015-106">修补特定的非安全策略有效负载。</span><span class="sxs-lookup"><span data-stu-id="de015-106">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de015-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="de015-107">Prerequisites</span></span>
<span data-ttu-id="de015-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de015-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="de015-110">Permission type</span></span>|<span data-ttu-id="de015-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de015-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de015-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de015-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de015-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de015-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de015-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de015-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de015-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de015-115">Not supported.</span></span>|
|<span data-ttu-id="de015-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="de015-116">Application</span></span>|<span data-ttu-id="de015-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="de015-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de015-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de015-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="de015-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="de015-119">Request headers</span></span>
|<span data-ttu-id="de015-120">标头</span><span class="sxs-lookup"><span data-stu-id="de015-120">Header</span></span>|<span data-ttu-id="de015-121">值</span><span class="sxs-lookup"><span data-stu-id="de015-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de015-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de015-122">Authorization</span></span>|<span data-ttu-id="de015-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de015-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de015-124">接受</span><span class="sxs-lookup"><span data-stu-id="de015-124">Accept</span></span>|<span data-ttu-id="de015-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de015-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de015-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="de015-126">Request body</span></span>
<span data-ttu-id="de015-127">在请求正文中, 提供[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de015-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="de015-128">下表显示创建[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de015-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="de015-129">属性</span><span class="sxs-lookup"><span data-stu-id="de015-129">Property</span></span>|<span data-ttu-id="de015-130">类型</span><span class="sxs-lookup"><span data-stu-id="de015-130">Type</span></span>|<span data-ttu-id="de015-131">说明</span><span class="sxs-lookup"><span data-stu-id="de015-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de015-132">id</span><span class="sxs-lookup"><span data-stu-id="de015-132">id</span></span>|<span data-ttu-id="de015-133">String</span><span class="sxs-lookup"><span data-stu-id="de015-133">String</span></span>|<span data-ttu-id="de015-134">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-134">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de015-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="de015-135">userPreferencePayload</span></span>|<span data-ttu-id="de015-136">Stream</span><span class="sxs-lookup"><span data-stu-id="de015-136">Stream</span></span>|<span data-ttu-id="de015-137">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-137">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de015-138">policyPayload</span><span class="sxs-lookup"><span data-stu-id="de015-138">policyPayload</span></span>|<span data-ttu-id="de015-139">Stream</span><span class="sxs-lookup"><span data-stu-id="de015-139">Stream</span></span>|<span data-ttu-id="de015-140">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-140">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de015-141">description</span><span class="sxs-lookup"><span data-stu-id="de015-141">description</span></span>|<span data-ttu-id="de015-142">字符串</span><span class="sxs-lookup"><span data-stu-id="de015-142">String</span></span>|<span data-ttu-id="de015-143">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-143">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de015-144">displayName</span><span class="sxs-lookup"><span data-stu-id="de015-144">displayName</span></span>|<span data-ttu-id="de015-145">String</span><span class="sxs-lookup"><span data-stu-id="de015-145">String</span></span>|<span data-ttu-id="de015-146">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-146">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de015-147">priority</span><span class="sxs-lookup"><span data-stu-id="de015-147">priority</span></span>|<span data-ttu-id="de015-148">Int32</span><span class="sxs-lookup"><span data-stu-id="de015-148">Int32</span></span>|<span data-ttu-id="de015-149">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-149">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de015-150">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="de015-150">userCheckinSummary</span></span>|[<span data-ttu-id="de015-151">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="de015-151">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="de015-152">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-152">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="de015-153">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="de015-153">checkinStatuses</span></span>|<span data-ttu-id="de015-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="de015-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="de015-155">尚未从[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)中继承的文档</span><span class="sxs-lookup"><span data-stu-id="de015-155">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="de015-156">响应</span><span class="sxs-lookup"><span data-stu-id="de015-156">Response</span></span>
<span data-ttu-id="de015-157">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de015-157">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de015-158">示例</span><span class="sxs-lookup"><span data-stu-id="de015-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="de015-159">请求</span><span class="sxs-lookup"><span data-stu-id="de015-159">Request</span></span>
<span data-ttu-id="de015-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de015-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de015-161">响应</span><span class="sxs-lookup"><span data-stu-id="de015-161">Response</span></span>
<span data-ttu-id="de015-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de015-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



