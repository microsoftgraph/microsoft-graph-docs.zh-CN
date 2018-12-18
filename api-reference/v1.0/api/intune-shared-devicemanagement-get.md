---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 65b13da27c16d6b4d9976eb2f7d0d326dfd872c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334334"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="5017c-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5017c-103">Get deviceManagement</span></span>

> <span data-ttu-id="5017c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5017c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5017c-105">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5017c-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5017c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5017c-106">Prerequisites</span></span>
<span data-ttu-id="5017c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5017c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5017c-109">权限&nbsp;类型&nbsp;(通过&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="5017c-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="5017c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5017c-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="5017c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5017c-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="5017c-112">&nbsp;&nbsp;审核</span><span class="sxs-lookup"><span data-stu-id="5017c-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="5017c-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="5017c-114">&nbsp;&nbsp;公司术语</span><span class="sxs-lookup"><span data-stu-id="5017c-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="5017c-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5017c-116">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="5017c-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="5017c-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5017c-118">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="5017c-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="5017c-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="5017c-120">&nbsp;&nbsp;注册</span><span class="sxs-lookup"><span data-stu-id="5017c-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="5017c-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5017c-122">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="5017c-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="5017c-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5017c-124">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="5017c-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="5017c-125">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5017c-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="5017c-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="5017c-127">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="5017c-128">&nbsp;&nbsp;远程协助</span><span class="sxs-lookup"><span data-stu-id="5017c-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="5017c-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5017c-130">&nbsp;&nbsp;电信支出管理</span><span class="sxs-lookup"><span data-stu-id="5017c-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="5017c-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5017c-132">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="5017c-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="5017c-133">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="5017c-134">&nbsp;&nbsp; Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="5017c-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="5017c-135">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017c-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="5017c-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5017c-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5017c-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="5017c-137">Not supported.</span></span>|
| <span data-ttu-id="5017c-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="5017c-138">Application</span></span> | <span data-ttu-id="5017c-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="5017c-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="5017c-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5017c-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5017c-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5017c-141">Optional query parameters</span></span>
<span data-ttu-id="5017c-142">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5017c-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5017c-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="5017c-143">Request headers</span></span>
|<span data-ttu-id="5017c-144">标头</span><span class="sxs-lookup"><span data-stu-id="5017c-144">Header</span></span>|<span data-ttu-id="5017c-145">值</span><span class="sxs-lookup"><span data-stu-id="5017c-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5017c-146">授权</span><span class="sxs-lookup"><span data-stu-id="5017c-146">Authorization</span></span>|<span data-ttu-id="5017c-147">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5017c-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5017c-148">Accept</span><span class="sxs-lookup"><span data-stu-id="5017c-148">Accept</span></span>|<span data-ttu-id="5017c-149">application/json</span><span class="sxs-lookup"><span data-stu-id="5017c-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5017c-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="5017c-150">Request body</span></span>
<span data-ttu-id="5017c-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5017c-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5017c-152">响应</span><span class="sxs-lookup"><span data-stu-id="5017c-152">Response</span></span>
<span data-ttu-id="5017c-153">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5017c-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5017c-154">示例</span><span class="sxs-lookup"><span data-stu-id="5017c-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="5017c-155">请求</span><span class="sxs-lookup"><span data-stu-id="5017c-155">Request</span></span>
<span data-ttu-id="5017c-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5017c-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="5017c-157">响应</span><span class="sxs-lookup"><span data-stu-id="5017c-157">Response</span></span>
<span data-ttu-id="5017c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5017c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



