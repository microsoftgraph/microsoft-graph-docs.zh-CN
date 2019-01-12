---
title: importAppleDeviceIdentityList 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c00279ecd56242d3b169a13e7018a6b5da9f182
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959648"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="aab66-103">importAppleDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="aab66-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="aab66-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aab66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aab66-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aab66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aab66-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aab66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aab66-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aab66-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aab66-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aab66-108">Prerequisites</span></span>
<span data-ttu-id="aab66-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="aab66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aab66-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aab66-111">Permission type</span></span>|<span data-ttu-id="aab66-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aab66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aab66-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aab66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aab66-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aab66-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aab66-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aab66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aab66-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aab66-116">Not supported.</span></span>|
|<span data-ttu-id="aab66-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aab66-117">Application</span></span>|<span data-ttu-id="aab66-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aab66-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aab66-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aab66-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="aab66-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aab66-120">Request headers</span></span>
|<span data-ttu-id="aab66-121">标头</span><span class="sxs-lookup"><span data-stu-id="aab66-121">Header</span></span>|<span data-ttu-id="aab66-122">值</span><span class="sxs-lookup"><span data-stu-id="aab66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aab66-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aab66-123">Authorization</span></span>|<span data-ttu-id="aab66-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aab66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aab66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aab66-125">Accept</span></span>|<span data-ttu-id="aab66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aab66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aab66-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aab66-127">Request body</span></span>
<span data-ttu-id="aab66-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aab66-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aab66-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="aab66-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aab66-130">属性</span><span class="sxs-lookup"><span data-stu-id="aab66-130">Property</span></span>|<span data-ttu-id="aab66-131">类型</span><span class="sxs-lookup"><span data-stu-id="aab66-131">Type</span></span>|<span data-ttu-id="aab66-132">说明</span><span class="sxs-lookup"><span data-stu-id="aab66-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aab66-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="aab66-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="aab66-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="aab66-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="aab66-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aab66-135">Not yet documented</span></span>|
|<span data-ttu-id="aab66-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="aab66-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="aab66-137">布尔</span><span class="sxs-lookup"><span data-stu-id="aab66-137">Boolean</span></span>|<span data-ttu-id="aab66-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aab66-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aab66-139">响应</span><span class="sxs-lookup"><span data-stu-id="aab66-139">Response</span></span>
<span data-ttu-id="aab66-140">如果成功，此操作将返回`200 OK`响应代码和响应正文中的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="aab66-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab66-141">示例</span><span class="sxs-lookup"><span data-stu-id="aab66-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="aab66-142">请求</span><span class="sxs-lookup"><span data-stu-id="aab66-142">Request</span></span>
<span data-ttu-id="aab66-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aab66-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aab66-144">响应</span><span class="sxs-lookup"><span data-stu-id="aab66-144">Response</span></span>
<span data-ttu-id="aab66-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aab66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





