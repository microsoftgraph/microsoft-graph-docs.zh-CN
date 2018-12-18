---
title: revokeDeviceLicense 操作
description: Revoke 分配 iOS VPP 设备许可证的给定应用程序。
author: tfitzmac
ms.openlocfilehash: 17ae2ed812d5c5b5a35926934d748fb730aafacf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353128"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="46d02-103">revokeDeviceLicense 操作</span><span class="sxs-lookup"><span data-stu-id="46d02-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="46d02-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="46d02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46d02-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="46d02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46d02-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="46d02-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46d02-107">Revoke 分配 iOS VPP 设备许可证的给定应用程序。</span><span class="sxs-lookup"><span data-stu-id="46d02-107">Revoke assigned iOS VPP device license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46d02-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="46d02-108">Prerequisites</span></span>
<span data-ttu-id="46d02-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="46d02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46d02-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="46d02-111">Permission type</span></span>|<span data-ttu-id="46d02-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46d02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46d02-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46d02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46d02-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d02-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46d02-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46d02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46d02-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d02-116">Not supported.</span></span>|
|<span data-ttu-id="46d02-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="46d02-117">Application</span></span>|<span data-ttu-id="46d02-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d02-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46d02-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46d02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="46d02-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="46d02-120">Request headers</span></span>
|<span data-ttu-id="46d02-121">标头</span><span class="sxs-lookup"><span data-stu-id="46d02-121">Header</span></span>|<span data-ttu-id="46d02-122">值</span><span class="sxs-lookup"><span data-stu-id="46d02-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46d02-123">授权</span><span class="sxs-lookup"><span data-stu-id="46d02-123">Authorization</span></span>|<span data-ttu-id="46d02-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46d02-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46d02-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46d02-125">Accept</span></span>|<span data-ttu-id="46d02-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46d02-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d02-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="46d02-127">Request body</span></span>
<span data-ttu-id="46d02-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46d02-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="46d02-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="46d02-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="46d02-130">属性</span><span class="sxs-lookup"><span data-stu-id="46d02-130">Property</span></span>|<span data-ttu-id="46d02-131">类型</span><span class="sxs-lookup"><span data-stu-id="46d02-131">Type</span></span>|<span data-ttu-id="46d02-132">说明</span><span class="sxs-lookup"><span data-stu-id="46d02-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46d02-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="46d02-133">managedDeviceId</span></span>|<span data-ttu-id="46d02-134">字符串</span><span class="sxs-lookup"><span data-stu-id="46d02-134">String</span></span>|<span data-ttu-id="46d02-135">为其分配的应用程序许可证是将撤消 DeviceId</span><span class="sxs-lookup"><span data-stu-id="46d02-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="46d02-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="46d02-136">notifyManagedDevices</span></span>|<span data-ttu-id="46d02-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="46d02-137">Boolean</span></span>|<span data-ttu-id="46d02-138">布尔值，指示 revoke 通知是否应发送给设备</span><span class="sxs-lookup"><span data-stu-id="46d02-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="46d02-139">响应</span><span class="sxs-lookup"><span data-stu-id="46d02-139">Response</span></span>
<span data-ttu-id="46d02-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="46d02-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="46d02-141">示例</span><span class="sxs-lookup"><span data-stu-id="46d02-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="46d02-142">请求</span><span class="sxs-lookup"><span data-stu-id="46d02-142">Request</span></span>
<span data-ttu-id="46d02-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46d02-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="46d02-144">响应</span><span class="sxs-lookup"><span data-stu-id="46d02-144">Response</span></span>
<span data-ttu-id="46d02-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46d02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





