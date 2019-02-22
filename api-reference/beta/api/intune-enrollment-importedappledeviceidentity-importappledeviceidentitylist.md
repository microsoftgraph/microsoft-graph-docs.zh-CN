---
title: importAppleDeviceIdentityList 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 714459b7ee5ab1dd65bb274ad2315e832ce56436
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141480"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="3f43c-103">importAppleDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="3f43c-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="3f43c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f43c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f43c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f43c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f43c-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f43c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f43c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f43c-107">Prerequisites</span></span>
<span data-ttu-id="3f43c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3f43c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3f43c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f43c-110">Permission type</span></span>|<span data-ttu-id="3f43c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3f43c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f43c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f43c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f43c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f43c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3f43c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f43c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f43c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f43c-115">Not supported.</span></span>|
|<span data-ttu-id="3f43c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f43c-116">Application</span></span>|<span data-ttu-id="3f43c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f43c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f43c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f43c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="3f43c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f43c-119">Request headers</span></span>
|<span data-ttu-id="3f43c-120">标头</span><span class="sxs-lookup"><span data-stu-id="3f43c-120">Header</span></span>|<span data-ttu-id="3f43c-121">值</span><span class="sxs-lookup"><span data-stu-id="3f43c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f43c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f43c-122">Authorization</span></span>|<span data-ttu-id="3f43c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f43c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f43c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3f43c-124">Accept</span></span>|<span data-ttu-id="3f43c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f43c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f43c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f43c-126">Request body</span></span>
<span data-ttu-id="3f43c-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f43c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3f43c-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="3f43c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3f43c-129">属性</span><span class="sxs-lookup"><span data-stu-id="3f43c-129">Property</span></span>|<span data-ttu-id="3f43c-130">类型</span><span class="sxs-lookup"><span data-stu-id="3f43c-130">Type</span></span>|<span data-ttu-id="3f43c-131">说明</span><span class="sxs-lookup"><span data-stu-id="3f43c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f43c-132">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3f43c-132">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="3f43c-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f43c-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="3f43c-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f43c-134">Not yet documented</span></span>|
|<span data-ttu-id="3f43c-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3f43c-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="3f43c-136">布尔</span><span class="sxs-lookup"><span data-stu-id="3f43c-136">Boolean</span></span>|<span data-ttu-id="3f43c-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f43c-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f43c-138">响应</span><span class="sxs-lookup"><span data-stu-id="3f43c-138">Response</span></span>
<span data-ttu-id="3f43c-139">如果成功, 此操作会在`200 OK`响应正文中返回响应代码和[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="3f43c-139">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f43c-140">示例</span><span class="sxs-lookup"><span data-stu-id="3f43c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f43c-141">请求</span><span class="sxs-lookup"><span data-stu-id="3f43c-141">Request</span></span>
<span data-ttu-id="3f43c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f43c-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 756

{
  "importedAppleDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
      "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="3f43c-143">响应</span><span class="sxs-lookup"><span data-stu-id="3f43c-143">Response</span></span>
<span data-ttu-id="3f43c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f43c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```




