---
title: revokeUserLicense 操作
description: Revoke 分配 iOS VPP 用户许可证的给定应用程序。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241306b812615bb804a3139082a439df9eeae059
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837301"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="5c5cb-103">revokeUserLicense 操作</span><span class="sxs-lookup"><span data-stu-id="5c5cb-103">revokeUserLicense action</span></span>

> <span data-ttu-id="5c5cb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c5cb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c5cb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c5cb-107">Revoke 分配 iOS VPP 用户许可证的给定应用程序。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-107">Revoke assigned iOS VPP user license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c5cb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c5cb-108">Prerequisites</span></span>
<span data-ttu-id="5c5cb-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5c5cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5cb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c5cb-111">Permission type</span></span>|<span data-ttu-id="5c5cb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5c5cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c5cb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c5cb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5cb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c5cb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c5cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-116">Not supported.</span></span>|
|<span data-ttu-id="5c5cb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c5cb-117">Application</span></span>|<span data-ttu-id="5c5cb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c5cb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c5cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="5c5cb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c5cb-120">Request headers</span></span>
|<span data-ttu-id="5c5cb-121">标头</span><span class="sxs-lookup"><span data-stu-id="5c5cb-121">Header</span></span>|<span data-ttu-id="5c5cb-122">值</span><span class="sxs-lookup"><span data-stu-id="5c5cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c5cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c5cb-123">Authorization</span></span>|<span data-ttu-id="5c5cb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c5cb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c5cb-125">Accept</span></span>|<span data-ttu-id="5c5cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c5cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c5cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c5cb-127">Request body</span></span>
<span data-ttu-id="5c5cb-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5c5cb-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5c5cb-130">属性</span><span class="sxs-lookup"><span data-stu-id="5c5cb-130">Property</span></span>|<span data-ttu-id="5c5cb-131">类型</span><span class="sxs-lookup"><span data-stu-id="5c5cb-131">Type</span></span>|<span data-ttu-id="5c5cb-132">Description</span><span class="sxs-lookup"><span data-stu-id="5c5cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c5cb-133">userId</span><span class="sxs-lookup"><span data-stu-id="5c5cb-133">userId</span></span>|<span data-ttu-id="5c5cb-134">String</span><span class="sxs-lookup"><span data-stu-id="5c5cb-134">String</span></span>|<span data-ttu-id="5c5cb-135">用户 Id 为其分配的应用程序许可证是将撤消</span><span class="sxs-lookup"><span data-stu-id="5c5cb-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="5c5cb-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="5c5cb-136">notifyManagedDevices</span></span>|<span data-ttu-id="5c5cb-137">布尔</span><span class="sxs-lookup"><span data-stu-id="5c5cb-137">Boolean</span></span>|<span data-ttu-id="5c5cb-138">布尔值，指示 revoke 通知是否应发送给设备</span><span class="sxs-lookup"><span data-stu-id="5c5cb-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="5c5cb-139">响应</span><span class="sxs-lookup"><span data-stu-id="5c5cb-139">Response</span></span>
<span data-ttu-id="5c5cb-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5c5cb-141">示例</span><span class="sxs-lookup"><span data-stu-id="5c5cb-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c5cb-142">请求</span><span class="sxs-lookup"><span data-stu-id="5c5cb-142">Request</span></span>
<span data-ttu-id="5c5cb-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="5c5cb-144">响应</span><span class="sxs-lookup"><span data-stu-id="5c5cb-144">Response</span></span>
<span data-ttu-id="5c5cb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c5cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





