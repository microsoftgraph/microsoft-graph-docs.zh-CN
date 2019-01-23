---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09563eeced6f557df2c2e40f126623f974cea2d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415864"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="098e9-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="098e9-103">Get deviceManagement</span></span>

> <span data-ttu-id="098e9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="098e9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="098e9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="098e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="098e9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="098e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="098e9-107">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="098e9-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="098e9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="098e9-108">Prerequisites</span></span>

<span data-ttu-id="098e9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="098e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="098e9-111">权限&nbsp;类型&nbsp;(通过&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="098e9-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="098e9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="098e9-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="098e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="098e9-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="098e9-114">&nbsp;&nbsp; **Android 的工时**</span><span class="sxs-lookup"><span data-stu-id="098e9-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="098e9-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="098e9-116">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="098e9-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="098e9-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="098e9-118">&nbsp;&nbsp; **公司术语**</span><span class="sxs-lookup"><span data-stu-id="098e9-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="098e9-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="098e9-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="098e9-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="098e9-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="098e9-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="098e9-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="098e9-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="098e9-124">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="098e9-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="098e9-125">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="098e9-126">&nbsp; &nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="098e9-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="098e9-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="098e9-128">&nbsp;&nbsp; **防御**</span><span class="sxs-lookup"><span data-stu-id="098e9-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="098e9-129">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="098e9-130">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="098e9-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="098e9-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="098e9-132">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="098e9-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="098e9-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="098e9-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="098e9-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="098e9-135">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="098e9-136">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="098e9-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="098e9-137">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="098e9-138">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="098e9-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="098e9-139">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="098e9-140">&nbsp;&nbsp; **电信支出管理**</span><span class="sxs-lookup"><span data-stu-id="098e9-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="098e9-141">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="098e9-142">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="098e9-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="098e9-143">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="098e9-144">&nbsp;&nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="098e9-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="098e9-145">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="098e9-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="098e9-146">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="098e9-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="098e9-147">不支持。</span><span class="sxs-lookup"><span data-stu-id="098e9-147">Not supported.</span></span>|
| <span data-ttu-id="098e9-148">应用程序</span><span class="sxs-lookup"><span data-stu-id="098e9-148">Application</span></span> | <span data-ttu-id="098e9-149">不支持。</span><span class="sxs-lookup"><span data-stu-id="098e9-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="098e9-150">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="098e9-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="098e9-151">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="098e9-151">Optional query parameters</span></span>

<span data-ttu-id="098e9-152">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="098e9-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="098e9-153">请求标头</span><span class="sxs-lookup"><span data-stu-id="098e9-153">Request headers</span></span>
|<span data-ttu-id="098e9-154">标头</span><span class="sxs-lookup"><span data-stu-id="098e9-154">Header</span></span>|<span data-ttu-id="098e9-155">值</span><span class="sxs-lookup"><span data-stu-id="098e9-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="098e9-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="098e9-156">Authorization</span></span>|<span data-ttu-id="098e9-157">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="098e9-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="098e9-158">Accept</span><span class="sxs-lookup"><span data-stu-id="098e9-158">Accept</span></span>|<span data-ttu-id="098e9-159">application/json</span><span class="sxs-lookup"><span data-stu-id="098e9-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="098e9-160">请求正文</span><span class="sxs-lookup"><span data-stu-id="098e9-160">Request body</span></span>

<span data-ttu-id="098e9-161">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="098e9-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="098e9-162">响应</span><span class="sxs-lookup"><span data-stu-id="098e9-162">Response</span></span>

<span data-ttu-id="098e9-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="098e9-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="098e9-164">示例</span><span class="sxs-lookup"><span data-stu-id="098e9-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="098e9-165">请求</span><span class="sxs-lookup"><span data-stu-id="098e9-165">Request</span></span>

<span data-ttu-id="098e9-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="098e9-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="098e9-167">响应</span><span class="sxs-lookup"><span data-stu-id="098e9-167">Response</span></span>

<span data-ttu-id="098e9-168">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="098e9-168">Here are example of the response.</span></span> 

<span data-ttu-id="098e9-169">注意： 为了简单起见，如下所示的响应对象可能被截断。</span><span class="sxs-lookup"><span data-stu-id="098e9-169">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="098e9-170">返回属性适用于工作流。</span><span class="sxs-lookup"><span data-stu-id="098e9-170">Properties appropriate for the workflow are returned.</span></span>

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



