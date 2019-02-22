---
title: revokeAllLicenses 操作
description: 为给定的应用程序吊销所有分配的 iOS VPP 许可证。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9850ff5ed3a3c9f382d0d2faa3a9cdcb97e3986
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169809"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="1fd52-103">revokeAllLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="1fd52-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="1fd52-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1fd52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fd52-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fd52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fd52-106">为给定的应用程序吊销所有分配的 iOS VPP 许可证。</span><span class="sxs-lookup"><span data-stu-id="1fd52-106">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fd52-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1fd52-107">Prerequisites</span></span>
<span data-ttu-id="1fd52-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1fd52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1fd52-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fd52-110">Permission type</span></span>|<span data-ttu-id="1fd52-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1fd52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fd52-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fd52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fd52-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd52-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1fd52-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fd52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fd52-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fd52-115">Not supported.</span></span>|
|<span data-ttu-id="1fd52-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fd52-116">Application</span></span>|<span data-ttu-id="1fd52-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fd52-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fd52-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="1fd52-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fd52-119">Request headers</span></span>
|<span data-ttu-id="1fd52-120">标头</span><span class="sxs-lookup"><span data-stu-id="1fd52-120">Header</span></span>|<span data-ttu-id="1fd52-121">值</span><span class="sxs-lookup"><span data-stu-id="1fd52-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fd52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fd52-122">Authorization</span></span>|<span data-ttu-id="1fd52-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1fd52-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fd52-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1fd52-124">Accept</span></span>|<span data-ttu-id="1fd52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1fd52-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd52-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fd52-126">Request body</span></span>
<span data-ttu-id="1fd52-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fd52-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1fd52-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1fd52-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1fd52-129">属性</span><span class="sxs-lookup"><span data-stu-id="1fd52-129">Property</span></span>|<span data-ttu-id="1fd52-130">类型</span><span class="sxs-lookup"><span data-stu-id="1fd52-130">Type</span></span>|<span data-ttu-id="1fd52-131">说明</span><span class="sxs-lookup"><span data-stu-id="1fd52-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fd52-132">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="1fd52-132">notifyManagedDevices</span></span>|<span data-ttu-id="1fd52-133">布尔</span><span class="sxs-lookup"><span data-stu-id="1fd52-133">Boolean</span></span>|<span data-ttu-id="1fd52-134">指示是否应将吊销通知发送到设备的布尔值</span><span class="sxs-lookup"><span data-stu-id="1fd52-134">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="1fd52-135">响应</span><span class="sxs-lookup"><span data-stu-id="1fd52-135">Response</span></span>
<span data-ttu-id="1fd52-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1fd52-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1fd52-137">示例</span><span class="sxs-lookup"><span data-stu-id="1fd52-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fd52-138">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-138">Request</span></span>
<span data-ttu-id="1fd52-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1fd52-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="1fd52-140">响应</span><span class="sxs-lookup"><span data-stu-id="1fd52-140">Response</span></span>
<span data-ttu-id="1fd52-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1fd52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




