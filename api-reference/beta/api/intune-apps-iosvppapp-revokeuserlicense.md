---
title: revokeUserLicense 操作
description: 撤销为给定应用分配的 iOS VPP 用户许可证。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfc1fa24858b4bddd76fca2d10f5d759d40c4797
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140637"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="15c05-103">revokeUserLicense 操作</span><span class="sxs-lookup"><span data-stu-id="15c05-103">revokeUserLicense action</span></span>

<span data-ttu-id="15c05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15c05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15c05-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="15c05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15c05-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="15c05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15c05-107">撤销为给定应用分配的 iOS VPP 用户许可证。</span><span class="sxs-lookup"><span data-stu-id="15c05-107">Revoke assigned iOS VPP user license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15c05-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="15c05-108">Prerequisites</span></span>
<span data-ttu-id="15c05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15c05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15c05-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="15c05-111">Permission type</span></span>|<span data-ttu-id="15c05-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15c05-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15c05-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15c05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15c05-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c05-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15c05-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15c05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15c05-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="15c05-116">Not supported.</span></span>|
|<span data-ttu-id="15c05-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="15c05-117">Application</span></span>|<span data-ttu-id="15c05-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c05-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15c05-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15c05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="15c05-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="15c05-120">Request headers</span></span>
|<span data-ttu-id="15c05-121">标头</span><span class="sxs-lookup"><span data-stu-id="15c05-121">Header</span></span>|<span data-ttu-id="15c05-122">值</span><span class="sxs-lookup"><span data-stu-id="15c05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15c05-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15c05-123">Authorization</span></span>|<span data-ttu-id="15c05-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="15c05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15c05-125">接受</span><span class="sxs-lookup"><span data-stu-id="15c05-125">Accept</span></span>|<span data-ttu-id="15c05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15c05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15c05-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="15c05-127">Request body</span></span>
<span data-ttu-id="15c05-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15c05-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="15c05-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="15c05-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="15c05-130">属性</span><span class="sxs-lookup"><span data-stu-id="15c05-130">Property</span></span>|<span data-ttu-id="15c05-131">类型</span><span class="sxs-lookup"><span data-stu-id="15c05-131">Type</span></span>|<span data-ttu-id="15c05-132">描述</span><span class="sxs-lookup"><span data-stu-id="15c05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c05-133">userId</span><span class="sxs-lookup"><span data-stu-id="15c05-133">userId</span></span>|<span data-ttu-id="15c05-134">String</span><span class="sxs-lookup"><span data-stu-id="15c05-134">String</span></span>|<span data-ttu-id="15c05-135">要吊销为其分配应用程序许可证的 UserId</span><span class="sxs-lookup"><span data-stu-id="15c05-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="15c05-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="15c05-136">notifyManagedDevices</span></span>|<span data-ttu-id="15c05-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="15c05-137">Boolean</span></span>|<span data-ttu-id="15c05-138">指示是否应当向设备发送撤销通知的布尔值</span><span class="sxs-lookup"><span data-stu-id="15c05-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="15c05-139">响应</span><span class="sxs-lookup"><span data-stu-id="15c05-139">Response</span></span>
<span data-ttu-id="15c05-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="15c05-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15c05-141">示例</span><span class="sxs-lookup"><span data-stu-id="15c05-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="15c05-142">请求</span><span class="sxs-lookup"><span data-stu-id="15c05-142">Request</span></span>
<span data-ttu-id="15c05-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="15c05-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="15c05-144">响应</span><span class="sxs-lookup"><span data-stu-id="15c05-144">Response</span></span>
<span data-ttu-id="15c05-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="15c05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




