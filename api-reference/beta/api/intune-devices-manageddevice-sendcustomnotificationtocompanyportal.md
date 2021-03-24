---
title: sendCustomNotificationToCompanyPortal 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0809f32ff83982f4964e68026f54872c6592be6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136270"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="e4268-103">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="e4268-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="e4268-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4268-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4268-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4268-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4268-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4268-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4268-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4268-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4268-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4268-108">Prerequisites</span></span>
<span data-ttu-id="e4268-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4268-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4268-111">Permission type</span></span>|<span data-ttu-id="e4268-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4268-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4268-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4268-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4268-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4268-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e4268-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4268-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4268-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4268-116">Not supported.</span></span>|
|<span data-ttu-id="e4268-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4268-117">Application</span></span>|<span data-ttu-id="e4268-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4268-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4268-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4268-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/comanagedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="e4268-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4268-120">Request headers</span></span>
|<span data-ttu-id="e4268-121">标头</span><span class="sxs-lookup"><span data-stu-id="e4268-121">Header</span></span>|<span data-ttu-id="e4268-122">值</span><span class="sxs-lookup"><span data-stu-id="e4268-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4268-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4268-123">Authorization</span></span>|<span data-ttu-id="e4268-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4268-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4268-125">接受</span><span class="sxs-lookup"><span data-stu-id="e4268-125">Accept</span></span>|<span data-ttu-id="e4268-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4268-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4268-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4268-127">Request body</span></span>
<span data-ttu-id="e4268-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4268-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e4268-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e4268-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e4268-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4268-130">Property</span></span>|<span data-ttu-id="e4268-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4268-131">Type</span></span>|<span data-ttu-id="e4268-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4268-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4268-133">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="e4268-133">notificationTitle</span></span>|<span data-ttu-id="e4268-134">String</span><span class="sxs-lookup"><span data-stu-id="e4268-134">String</span></span>|<span data-ttu-id="e4268-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4268-135">Not yet documented</span></span>|
|<span data-ttu-id="e4268-136">notificationBody</span><span class="sxs-lookup"><span data-stu-id="e4268-136">notificationBody</span></span>|<span data-ttu-id="e4268-137">String</span><span class="sxs-lookup"><span data-stu-id="e4268-137">String</span></span>|<span data-ttu-id="e4268-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4268-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e4268-139">响应</span><span class="sxs-lookup"><span data-stu-id="e4268-139">Response</span></span>
<span data-ttu-id="e4268-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e4268-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4268-141">示例</span><span class="sxs-lookup"><span data-stu-id="e4268-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4268-142">请求</span><span class="sxs-lookup"><span data-stu-id="e4268-142">Request</span></span>
<span data-ttu-id="e4268-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4268-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 105

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="e4268-144">响应</span><span class="sxs-lookup"><span data-stu-id="e4268-144">Response</span></span>
<span data-ttu-id="e4268-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4268-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




