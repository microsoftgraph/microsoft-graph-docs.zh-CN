---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd689c80863504e5ae3766a11684a83ed89d086b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361467"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="02808-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="02808-103">Get deviceManagement</span></span>

> <span data-ttu-id="02808-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02808-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02808-105">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="02808-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02808-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="02808-106">Prerequisites</span></span>
<span data-ttu-id="02808-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02808-109">权限&nbsp;类型&nbsp;（按&nbsp;工作流）</span><span class="sxs-lookup"><span data-stu-id="02808-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="02808-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02808-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="02808-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02808-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="02808-112">&nbsp;&nbsp;审核</span><span class="sxs-lookup"><span data-stu-id="02808-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="02808-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="02808-114">&nbsp;&nbsp;公司条款</span><span class="sxs-lookup"><span data-stu-id="02808-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="02808-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="02808-116">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="02808-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="02808-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="02808-118">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="02808-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="02808-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="02808-120">&nbsp;&nbsp;注册</span><span class="sxs-lookup"><span data-stu-id="02808-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="02808-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="02808-122">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="02808-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="02808-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="02808-124">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="02808-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="02808-125">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="02808-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="02808-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="02808-127">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="02808-128">&nbsp;&nbsp;远程协助</span><span class="sxs-lookup"><span data-stu-id="02808-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="02808-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="02808-130">&nbsp;&nbsp;电信费用管理</span><span class="sxs-lookup"><span data-stu-id="02808-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="02808-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="02808-132">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="02808-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="02808-133">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="02808-134">&nbsp;&nbsp; Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="02808-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="02808-135">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02808-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="02808-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02808-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02808-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="02808-137">Not supported.</span></span>|
| <span data-ttu-id="02808-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="02808-138">Application</span></span> | <span data-ttu-id="02808-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="02808-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="02808-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02808-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02808-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="02808-141">Optional query parameters</span></span>
<span data-ttu-id="02808-142">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="02808-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="02808-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="02808-143">Request headers</span></span>
|<span data-ttu-id="02808-144">标头</span><span class="sxs-lookup"><span data-stu-id="02808-144">Header</span></span>|<span data-ttu-id="02808-145">值</span><span class="sxs-lookup"><span data-stu-id="02808-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02808-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="02808-146">Authorization</span></span>|<span data-ttu-id="02808-147">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="02808-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02808-148">接受</span><span class="sxs-lookup"><span data-stu-id="02808-148">Accept</span></span>|<span data-ttu-id="02808-149">application/json</span><span class="sxs-lookup"><span data-stu-id="02808-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02808-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="02808-150">Request body</span></span>
<span data-ttu-id="02808-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02808-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02808-152">响应</span><span class="sxs-lookup"><span data-stu-id="02808-152">Response</span></span>
<span data-ttu-id="02808-153">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02808-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02808-154">示例</span><span class="sxs-lookup"><span data-stu-id="02808-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="02808-155">请求</span><span class="sxs-lookup"><span data-stu-id="02808-155">Request</span></span>
<span data-ttu-id="02808-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02808-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="02808-157">响应</span><span class="sxs-lookup"><span data-stu-id="02808-157">Response</span></span>
<span data-ttu-id="02808-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02808-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




