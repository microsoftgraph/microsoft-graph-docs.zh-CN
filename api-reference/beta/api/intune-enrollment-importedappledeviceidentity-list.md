---
title: 列表 importedAppleDeviceIdentities
description: 列出属性和 importedAppleDeviceIdentity 对象之间的关系。
ms.openlocfilehash: b0b490f6c3de9166bbbd497a819cd3799eef6cff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044398"
---
# <a name="list-importedappledeviceidentities"></a><span data-ttu-id="86343-103">列表 importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="86343-103">List importedAppleDeviceIdentities</span></span>

> <span data-ttu-id="86343-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="86343-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86343-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86343-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86343-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="86343-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86343-107">列出属性和[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="86343-107">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86343-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="86343-108">Prerequisites</span></span>
<span data-ttu-id="86343-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="86343-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86343-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="86343-111">Permission type</span></span>|<span data-ttu-id="86343-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86343-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86343-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86343-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86343-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="86343-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="86343-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86343-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86343-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86343-116">Not supported.</span></span>|
|<span data-ttu-id="86343-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86343-117">Application</span></span>|<span data-ttu-id="86343-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="86343-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86343-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86343-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="86343-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86343-120">Request headers</span></span>
|<span data-ttu-id="86343-121">标头</span><span class="sxs-lookup"><span data-stu-id="86343-121">Header</span></span>|<span data-ttu-id="86343-122">值</span><span class="sxs-lookup"><span data-stu-id="86343-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86343-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86343-123">Authorization</span></span>|<span data-ttu-id="86343-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86343-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86343-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86343-125">Accept</span></span>|<span data-ttu-id="86343-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86343-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86343-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86343-127">Request body</span></span>
<span data-ttu-id="86343-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86343-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86343-129">响应</span><span class="sxs-lookup"><span data-stu-id="86343-129">Response</span></span>
<span data-ttu-id="86343-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="86343-130">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86343-131">示例</span><span class="sxs-lookup"><span data-stu-id="86343-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="86343-132">请求</span><span class="sxs-lookup"><span data-stu-id="86343-132">Request</span></span>
<span data-ttu-id="86343-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86343-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="86343-134">响应</span><span class="sxs-lookup"><span data-stu-id="86343-134">Response</span></span>
<span data-ttu-id="86343-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86343-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
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
  ]
}
```





