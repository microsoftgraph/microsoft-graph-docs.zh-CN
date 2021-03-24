---
title: revokeDeviceLicense 操作
description: 撤销为给定应用分配的 iOS VPP 设备许可证。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 648677f00c26c4432614eda9ce840b152528a5e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144100"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="8c6e1-103">revokeDeviceLicense 操作</span><span class="sxs-lookup"><span data-stu-id="8c6e1-103">revokeDeviceLicense action</span></span>

<span data-ttu-id="8c6e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c6e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c6e1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c6e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c6e1-107">撤销为给定应用分配的 iOS VPP 设备许可证。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-107">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c6e1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c6e1-108">Prerequisites</span></span>
<span data-ttu-id="8c6e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c6e1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c6e1-111">Permission type</span></span>|<span data-ttu-id="8c6e1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c6e1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c6e1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c6e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c6e1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c6e1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c6e1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c6e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c6e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-116">Not supported.</span></span>|
|<span data-ttu-id="8c6e1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c6e1-117">Application</span></span>|<span data-ttu-id="8c6e1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c6e1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c6e1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c6e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="8c6e1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c6e1-120">Request headers</span></span>
|<span data-ttu-id="8c6e1-121">标头</span><span class="sxs-lookup"><span data-stu-id="8c6e1-121">Header</span></span>|<span data-ttu-id="8c6e1-122">值</span><span class="sxs-lookup"><span data-stu-id="8c6e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c6e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c6e1-123">Authorization</span></span>|<span data-ttu-id="8c6e1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c6e1-125">接受</span><span class="sxs-lookup"><span data-stu-id="8c6e1-125">Accept</span></span>|<span data-ttu-id="8c6e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c6e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c6e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c6e1-127">Request body</span></span>
<span data-ttu-id="8c6e1-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8c6e1-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8c6e1-130">属性</span><span class="sxs-lookup"><span data-stu-id="8c6e1-130">Property</span></span>|<span data-ttu-id="8c6e1-131">类型</span><span class="sxs-lookup"><span data-stu-id="8c6e1-131">Type</span></span>|<span data-ttu-id="8c6e1-132">说明</span><span class="sxs-lookup"><span data-stu-id="8c6e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c6e1-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8c6e1-133">managedDeviceId</span></span>|<span data-ttu-id="8c6e1-134">String</span><span class="sxs-lookup"><span data-stu-id="8c6e1-134">String</span></span>|<span data-ttu-id="8c6e1-135">要吊销为其分配应用许可证的 DeviceId</span><span class="sxs-lookup"><span data-stu-id="8c6e1-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="8c6e1-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="8c6e1-136">notifyManagedDevices</span></span>|<span data-ttu-id="8c6e1-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c6e1-137">Boolean</span></span>|<span data-ttu-id="8c6e1-138">指示是否应当向设备发送撤销通知的布尔值</span><span class="sxs-lookup"><span data-stu-id="8c6e1-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="8c6e1-139">响应</span><span class="sxs-lookup"><span data-stu-id="8c6e1-139">Response</span></span>
<span data-ttu-id="8c6e1-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c6e1-141">示例</span><span class="sxs-lookup"><span data-stu-id="8c6e1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c6e1-142">请求</span><span class="sxs-lookup"><span data-stu-id="8c6e1-142">Request</span></span>
<span data-ttu-id="8c6e1-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="8c6e1-144">响应</span><span class="sxs-lookup"><span data-stu-id="8c6e1-144">Response</span></span>
<span data-ttu-id="8c6e1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c6e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




