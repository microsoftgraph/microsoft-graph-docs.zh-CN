---
title: 删除 microsoftStoreForBusinessApp
description: 删除 microsoftStoreForBusinessApp。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55da404c8375958b1c09dd18d57acc52c436b86e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974382"
---
# <a name="delete-microsoftstoreforbusinessapp"></a><span data-ttu-id="bf577-103">删除 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="bf577-103">Delete microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="bf577-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf577-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf577-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf577-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf577-106">删除 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)。</span><span class="sxs-lookup"><span data-stu-id="bf577-106">Deletes a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf577-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf577-107">Prerequisites</span></span>
<span data-ttu-id="bf577-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf577-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf577-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf577-110">Permission type</span></span>|<span data-ttu-id="bf577-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf577-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf577-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf577-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf577-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf577-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bf577-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf577-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf577-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf577-115">Not supported.</span></span>|
|<span data-ttu-id="bf577-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf577-116">Application</span></span>|<span data-ttu-id="bf577-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf577-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf577-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf577-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bf577-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf577-119">Request headers</span></span>
|<span data-ttu-id="bf577-120">标头</span><span class="sxs-lookup"><span data-stu-id="bf577-120">Header</span></span>|<span data-ttu-id="bf577-121">值</span><span class="sxs-lookup"><span data-stu-id="bf577-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf577-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf577-122">Authorization</span></span>|<span data-ttu-id="bf577-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf577-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf577-124">接受</span><span class="sxs-lookup"><span data-stu-id="bf577-124">Accept</span></span>|<span data-ttu-id="bf577-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf577-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf577-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf577-126">Request body</span></span>
<span data-ttu-id="bf577-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bf577-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf577-128">响应</span><span class="sxs-lookup"><span data-stu-id="bf577-128">Response</span></span>
<span data-ttu-id="bf577-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bf577-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf577-130">示例</span><span class="sxs-lookup"><span data-stu-id="bf577-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf577-131">请求</span><span class="sxs-lookup"><span data-stu-id="bf577-131">Request</span></span>
<span data-ttu-id="bf577-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf577-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="bf577-133">响应</span><span class="sxs-lookup"><span data-stu-id="bf577-133">Response</span></span>
<span data-ttu-id="bf577-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf577-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





