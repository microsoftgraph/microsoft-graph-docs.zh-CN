---
title: revokeUserLicense 操作
description: 为给定应用撤销分配的 iOS VPP 用户许可证。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 662f71488d3fcafbe60578992c133a693ae729e1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172973"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="9bb58-103">revokeUserLicense 操作</span><span class="sxs-lookup"><span data-stu-id="9bb58-103">revokeUserLicense action</span></span>

> <span data-ttu-id="9bb58-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9bb58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bb58-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9bb58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bb58-106">为给定应用撤销分配的 iOS VPP 用户许可证。</span><span class="sxs-lookup"><span data-stu-id="9bb58-106">Revoke assigned iOS VPP user license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bb58-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9bb58-107">Prerequisites</span></span>
<span data-ttu-id="9bb58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9bb58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9bb58-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bb58-110">Permission type</span></span>|<span data-ttu-id="9bb58-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9bb58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bb58-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bb58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bb58-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bb58-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9bb58-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bb58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bb58-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bb58-115">Not supported.</span></span>|
|<span data-ttu-id="9bb58-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bb58-116">Application</span></span>|<span data-ttu-id="9bb58-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bb58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bb58-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bb58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="9bb58-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bb58-119">Request headers</span></span>
|<span data-ttu-id="9bb58-120">标头</span><span class="sxs-lookup"><span data-stu-id="9bb58-120">Header</span></span>|<span data-ttu-id="9bb58-121">值</span><span class="sxs-lookup"><span data-stu-id="9bb58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bb58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bb58-122">Authorization</span></span>|<span data-ttu-id="9bb58-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9bb58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bb58-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9bb58-124">Accept</span></span>|<span data-ttu-id="9bb58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bb58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb58-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bb58-126">Request body</span></span>
<span data-ttu-id="9bb58-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bb58-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9bb58-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9bb58-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9bb58-129">属性</span><span class="sxs-lookup"><span data-stu-id="9bb58-129">Property</span></span>|<span data-ttu-id="9bb58-130">类型</span><span class="sxs-lookup"><span data-stu-id="9bb58-130">Type</span></span>|<span data-ttu-id="9bb58-131">说明</span><span class="sxs-lookup"><span data-stu-id="9bb58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb58-132">userId</span><span class="sxs-lookup"><span data-stu-id="9bb58-132">userId</span></span>|<span data-ttu-id="9bb58-133">String</span><span class="sxs-lookup"><span data-stu-id="9bb58-133">String</span></span>|<span data-ttu-id="9bb58-134">要吊销的已分配应用程序许可证的用户 id</span><span class="sxs-lookup"><span data-stu-id="9bb58-134">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="9bb58-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="9bb58-135">notifyManagedDevices</span></span>|<span data-ttu-id="9bb58-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bb58-136">Boolean</span></span>|<span data-ttu-id="9bb58-137">指示是否应将吊销通知发送到设备的布尔值</span><span class="sxs-lookup"><span data-stu-id="9bb58-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="9bb58-138">响应</span><span class="sxs-lookup"><span data-stu-id="9bb58-138">Response</span></span>
<span data-ttu-id="9bb58-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9bb58-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9bb58-140">示例</span><span class="sxs-lookup"><span data-stu-id="9bb58-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bb58-141">请求</span><span class="sxs-lookup"><span data-stu-id="9bb58-141">Request</span></span>
<span data-ttu-id="9bb58-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9bb58-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="9bb58-143">响应</span><span class="sxs-lookup"><span data-stu-id="9bb58-143">Response</span></span>
<span data-ttu-id="9bb58-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bb58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




