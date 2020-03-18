---
title: 删除 androidManagedAppProtection
description: 删除 androidManagedAppProtection。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58c802968a9fed2b1f93e4be8f1cda4562e28105
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801304"
---
# <a name="delete-androidmanagedappprotection"></a><span data-ttu-id="e3903-103">删除 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="e3903-103">Delete androidManagedAppProtection</span></span>

> <span data-ttu-id="e3903-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3903-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3903-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3903-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3903-106">删除 [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="e3903-106">Deletes a [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3903-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e3903-107">Prerequisites</span></span>
<span data-ttu-id="e3903-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3903-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3903-110">Permission type</span></span>|<span data-ttu-id="e3903-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e3903-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3903-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3903-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e3903-113">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="e3903-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="e3903-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3903-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="e3903-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="e3903-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e3903-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3903-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3903-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3903-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3903-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3903-118">Not supported.</span></span>|
|<span data-ttu-id="e3903-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3903-119">Application</span></span>||
| <span data-ttu-id="e3903-120">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="e3903-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="e3903-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3903-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="e3903-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="e3903-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e3903-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3903-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3903-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3903-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="e3903-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3903-125">Request headers</span></span>
|<span data-ttu-id="e3903-126">标头</span><span class="sxs-lookup"><span data-stu-id="e3903-126">Header</span></span>|<span data-ttu-id="e3903-127">值</span><span class="sxs-lookup"><span data-stu-id="e3903-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3903-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3903-128">Authorization</span></span>|<span data-ttu-id="e3903-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e3903-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3903-130">接受</span><span class="sxs-lookup"><span data-stu-id="e3903-130">Accept</span></span>|<span data-ttu-id="e3903-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e3903-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3903-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3903-132">Request body</span></span>
<span data-ttu-id="e3903-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3903-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3903-134">响应</span><span class="sxs-lookup"><span data-stu-id="e3903-134">Response</span></span>
<span data-ttu-id="e3903-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e3903-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e3903-136">示例</span><span class="sxs-lookup"><span data-stu-id="e3903-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3903-137">请求</span><span class="sxs-lookup"><span data-stu-id="e3903-137">Request</span></span>
<span data-ttu-id="e3903-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3903-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="e3903-139">响应</span><span class="sxs-lookup"><span data-stu-id="e3903-139">Response</span></span>
<span data-ttu-id="e3903-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3903-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







