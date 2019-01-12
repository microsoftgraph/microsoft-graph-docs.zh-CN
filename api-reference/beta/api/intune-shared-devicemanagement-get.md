---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 689a06d94b7ec0af267b4fa5af7df5e31e34491d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945494"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="998ef-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="998ef-103">Get deviceManagement</span></span>

> <span data-ttu-id="998ef-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="998ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="998ef-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="998ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="998ef-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="998ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="998ef-107">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="998ef-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="998ef-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="998ef-108">Prerequisites</span></span>

<span data-ttu-id="998ef-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="998ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="998ef-111">权限&nbsp;类型&nbsp;(通过&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="998ef-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="998ef-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="998ef-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="998ef-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="998ef-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="998ef-114">&nbsp;&nbsp; **Android 的工时**</span><span class="sxs-lookup"><span data-stu-id="998ef-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="998ef-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="998ef-116">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="998ef-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="998ef-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="998ef-118">&nbsp;&nbsp; **公司术语**</span><span class="sxs-lookup"><span data-stu-id="998ef-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="998ef-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="998ef-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="998ef-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="998ef-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="998ef-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="998ef-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="998ef-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="998ef-124">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="998ef-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="998ef-125">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="998ef-126">&nbsp; &nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="998ef-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="998ef-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="998ef-128">&nbsp;&nbsp; **防御**</span><span class="sxs-lookup"><span data-stu-id="998ef-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="998ef-129">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="998ef-130">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="998ef-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="998ef-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="998ef-132">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="998ef-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="998ef-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="998ef-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="998ef-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="998ef-135">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="998ef-136">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="998ef-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="998ef-137">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="998ef-138">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="998ef-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="998ef-139">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="998ef-140">&nbsp;&nbsp; **电信支出管理**</span><span class="sxs-lookup"><span data-stu-id="998ef-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="998ef-141">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="998ef-142">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="998ef-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="998ef-143">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="998ef-144">&nbsp;&nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="998ef-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="998ef-145">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="998ef-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="998ef-146">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="998ef-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="998ef-147">不支持。</span><span class="sxs-lookup"><span data-stu-id="998ef-147">Not supported.</span></span>|
| <span data-ttu-id="998ef-148">应用程序</span><span class="sxs-lookup"><span data-stu-id="998ef-148">Application</span></span> | <span data-ttu-id="998ef-149">不支持。</span><span class="sxs-lookup"><span data-stu-id="998ef-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="998ef-150">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="998ef-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="998ef-151">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="998ef-151">Optional query parameters</span></span>

<span data-ttu-id="998ef-152">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="998ef-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="998ef-153">请求标头</span><span class="sxs-lookup"><span data-stu-id="998ef-153">Request headers</span></span>
|<span data-ttu-id="998ef-154">标头</span><span class="sxs-lookup"><span data-stu-id="998ef-154">Header</span></span>|<span data-ttu-id="998ef-155">值</span><span class="sxs-lookup"><span data-stu-id="998ef-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="998ef-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="998ef-156">Authorization</span></span>|<span data-ttu-id="998ef-157">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="998ef-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="998ef-158">Accept</span><span class="sxs-lookup"><span data-stu-id="998ef-158">Accept</span></span>|<span data-ttu-id="998ef-159">application/json</span><span class="sxs-lookup"><span data-stu-id="998ef-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="998ef-160">请求正文</span><span class="sxs-lookup"><span data-stu-id="998ef-160">Request body</span></span>

<span data-ttu-id="998ef-161">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="998ef-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="998ef-162">响应</span><span class="sxs-lookup"><span data-stu-id="998ef-162">Response</span></span>

<span data-ttu-id="998ef-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="998ef-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="998ef-164">示例</span><span class="sxs-lookup"><span data-stu-id="998ef-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="998ef-165">请求</span><span class="sxs-lookup"><span data-stu-id="998ef-165">Request</span></span>

<span data-ttu-id="998ef-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="998ef-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="998ef-167">响应</span><span class="sxs-lookup"><span data-stu-id="998ef-167">Response</span></span>

<span data-ttu-id="998ef-168">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="998ef-168">Here are example of the response.</span></span> 

<span data-ttu-id="998ef-169">注意： 为了简单起见，如下所示的响应对象可能被截断。</span><span class="sxs-lookup"><span data-stu-id="998ef-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="998ef-170">返回属性适用于工作流。</span><span class="sxs-lookup"><span data-stu-id="998ef-170">Properties appropriate for the workflow are returned.</span></span>

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



