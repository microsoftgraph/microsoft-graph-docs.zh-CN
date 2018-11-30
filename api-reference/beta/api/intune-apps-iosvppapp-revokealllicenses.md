---
title: revokeAllLicenses 操作
description: Revoke 所有分配 iOS 给定应用程序的许可 VPP。
ms.openlocfilehash: 576cbf5b63f9eb1f00a409483a36a483bf0c9892
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048717"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="37d0e-103">revokeAllLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="37d0e-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="37d0e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="37d0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37d0e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37d0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37d0e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="37d0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37d0e-107">Revoke 所有分配 iOS 给定应用程序的许可 VPP。</span><span class="sxs-lookup"><span data-stu-id="37d0e-107">Revoke all assigned iOS VPP licenses for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37d0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="37d0e-108">Prerequisites</span></span>
<span data-ttu-id="37d0e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="37d0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37d0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="37d0e-111">Permission type</span></span>|<span data-ttu-id="37d0e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="37d0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37d0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37d0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37d0e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d0e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37d0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37d0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37d0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37d0e-116">Not supported.</span></span>|
|<span data-ttu-id="37d0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="37d0e-117">Application</span></span>|<span data-ttu-id="37d0e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="37d0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37d0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37d0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="37d0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="37d0e-120">Request headers</span></span>
|<span data-ttu-id="37d0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="37d0e-121">Header</span></span>|<span data-ttu-id="37d0e-122">值</span><span class="sxs-lookup"><span data-stu-id="37d0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37d0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37d0e-123">Authorization</span></span>|<span data-ttu-id="37d0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37d0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37d0e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37d0e-125">Accept</span></span>|<span data-ttu-id="37d0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37d0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37d0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37d0e-127">Request body</span></span>
<span data-ttu-id="37d0e-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37d0e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="37d0e-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="37d0e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="37d0e-130">属性</span><span class="sxs-lookup"><span data-stu-id="37d0e-130">Property</span></span>|<span data-ttu-id="37d0e-131">类型</span><span class="sxs-lookup"><span data-stu-id="37d0e-131">Type</span></span>|<span data-ttu-id="37d0e-132">说明</span><span class="sxs-lookup"><span data-stu-id="37d0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d0e-133">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="37d0e-133">notifyManagedDevices</span></span>|<span data-ttu-id="37d0e-134">布尔</span><span class="sxs-lookup"><span data-stu-id="37d0e-134">Boolean</span></span>|<span data-ttu-id="37d0e-135">布尔值，指示 revoke 通知是否应发送给设备</span><span class="sxs-lookup"><span data-stu-id="37d0e-135">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="37d0e-136">响应</span><span class="sxs-lookup"><span data-stu-id="37d0e-136">Response</span></span>
<span data-ttu-id="37d0e-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="37d0e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="37d0e-138">示例</span><span class="sxs-lookup"><span data-stu-id="37d0e-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="37d0e-139">请求</span><span class="sxs-lookup"><span data-stu-id="37d0e-139">Request</span></span>
<span data-ttu-id="37d0e-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37d0e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="37d0e-141">响应</span><span class="sxs-lookup"><span data-stu-id="37d0e-141">Response</span></span>
<span data-ttu-id="37d0e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37d0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





