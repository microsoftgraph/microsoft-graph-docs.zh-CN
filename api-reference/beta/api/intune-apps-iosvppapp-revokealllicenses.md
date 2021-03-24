---
title: revokeAllLicenses 操作
description: 撤销给定应用的所有分配 iOS VPP 许可证。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13c4dcd973d7dc14141097056ccbd6c11608dad2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140677"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="13bd4-103">revokeAllLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="13bd4-103">revokeAllLicenses action</span></span>

<span data-ttu-id="13bd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13bd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13bd4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13bd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13bd4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13bd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13bd4-107">撤销给定应用的所有分配 iOS VPP 许可证。</span><span class="sxs-lookup"><span data-stu-id="13bd4-107">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13bd4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="13bd4-108">Prerequisites</span></span>
<span data-ttu-id="13bd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13bd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13bd4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="13bd4-111">Permission type</span></span>|<span data-ttu-id="13bd4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13bd4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13bd4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13bd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13bd4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bd4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13bd4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13bd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13bd4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="13bd4-116">Not supported.</span></span>|
|<span data-ttu-id="13bd4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="13bd4-117">Application</span></span>|<span data-ttu-id="13bd4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bd4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13bd4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13bd4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="13bd4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="13bd4-120">Request headers</span></span>
|<span data-ttu-id="13bd4-121">标头</span><span class="sxs-lookup"><span data-stu-id="13bd4-121">Header</span></span>|<span data-ttu-id="13bd4-122">值</span><span class="sxs-lookup"><span data-stu-id="13bd4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13bd4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13bd4-123">Authorization</span></span>|<span data-ttu-id="13bd4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="13bd4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13bd4-125">接受</span><span class="sxs-lookup"><span data-stu-id="13bd4-125">Accept</span></span>|<span data-ttu-id="13bd4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13bd4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13bd4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="13bd4-127">Request body</span></span>
<span data-ttu-id="13bd4-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13bd4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="13bd4-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="13bd4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="13bd4-130">属性</span><span class="sxs-lookup"><span data-stu-id="13bd4-130">Property</span></span>|<span data-ttu-id="13bd4-131">类型</span><span class="sxs-lookup"><span data-stu-id="13bd4-131">Type</span></span>|<span data-ttu-id="13bd4-132">说明</span><span class="sxs-lookup"><span data-stu-id="13bd4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bd4-133">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="13bd4-133">notifyManagedDevices</span></span>|<span data-ttu-id="13bd4-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="13bd4-134">Boolean</span></span>|<span data-ttu-id="13bd4-135">指示是否应当向设备发送撤销通知的布尔值</span><span class="sxs-lookup"><span data-stu-id="13bd4-135">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="13bd4-136">响应</span><span class="sxs-lookup"><span data-stu-id="13bd4-136">Response</span></span>
<span data-ttu-id="13bd4-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="13bd4-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13bd4-138">示例</span><span class="sxs-lookup"><span data-stu-id="13bd4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="13bd4-139">请求</span><span class="sxs-lookup"><span data-stu-id="13bd4-139">Request</span></span>
<span data-ttu-id="13bd4-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13bd4-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="13bd4-141">响应</span><span class="sxs-lookup"><span data-stu-id="13bd4-141">Response</span></span>
<span data-ttu-id="13bd4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13bd4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




