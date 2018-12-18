---
title: importAppleDeviceIdentityList 操作
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 9ddd4ea6be25faaba089ee8e8d8b9a40edfbf9a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325492"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="87ca7-103">importAppleDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="87ca7-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="87ca7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="87ca7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87ca7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="87ca7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87ca7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="87ca7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87ca7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="87ca7-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87ca7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="87ca7-108">Prerequisites</span></span>
<span data-ttu-id="87ca7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="87ca7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ca7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87ca7-111">Permission type</span></span>|<span data-ttu-id="87ca7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="87ca7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87ca7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87ca7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87ca7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ca7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="87ca7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87ca7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87ca7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87ca7-116">Not supported.</span></span>|
|<span data-ttu-id="87ca7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87ca7-117">Application</span></span>|<span data-ttu-id="87ca7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="87ca7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87ca7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87ca7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="87ca7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="87ca7-120">Request headers</span></span>
|<span data-ttu-id="87ca7-121">标头</span><span class="sxs-lookup"><span data-stu-id="87ca7-121">Header</span></span>|<span data-ttu-id="87ca7-122">值</span><span class="sxs-lookup"><span data-stu-id="87ca7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87ca7-123">授权</span><span class="sxs-lookup"><span data-stu-id="87ca7-123">Authorization</span></span>|<span data-ttu-id="87ca7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87ca7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87ca7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87ca7-125">Accept</span></span>|<span data-ttu-id="87ca7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87ca7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87ca7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="87ca7-127">Request body</span></span>
<span data-ttu-id="87ca7-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87ca7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="87ca7-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="87ca7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="87ca7-130">属性</span><span class="sxs-lookup"><span data-stu-id="87ca7-130">Property</span></span>|<span data-ttu-id="87ca7-131">类型</span><span class="sxs-lookup"><span data-stu-id="87ca7-131">Type</span></span>|<span data-ttu-id="87ca7-132">说明</span><span class="sxs-lookup"><span data-stu-id="87ca7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ca7-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="87ca7-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="87ca7-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="87ca7-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="87ca7-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="87ca7-135">Not yet documented</span></span>|
|<span data-ttu-id="87ca7-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="87ca7-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="87ca7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ca7-137">Boolean</span></span>|<span data-ttu-id="87ca7-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="87ca7-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="87ca7-139">响应</span><span class="sxs-lookup"><span data-stu-id="87ca7-139">Response</span></span>
<span data-ttu-id="87ca7-140">如果成功，此操作将返回`200 OK`响应代码和响应正文中的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="87ca7-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ca7-141">示例</span><span class="sxs-lookup"><span data-stu-id="87ca7-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="87ca7-142">请求</span><span class="sxs-lookup"><span data-stu-id="87ca7-142">Request</span></span>
<span data-ttu-id="87ca7-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87ca7-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="87ca7-144">响应</span><span class="sxs-lookup"><span data-stu-id="87ca7-144">Response</span></span>
<span data-ttu-id="87ca7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87ca7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





