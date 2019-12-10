---
title: 删除 windowsStoreApp
description: 删除 windowsStoreApp。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc970846a12a01bff221408c0bb781c7e126c3d3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39932724"
---
# <a name="delete-windowsstoreapp"></a><span data-ttu-id="17a11-103">删除 windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="17a11-103">Delete windowsStoreApp</span></span>

> <span data-ttu-id="17a11-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17a11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17a11-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17a11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17a11-106">删除[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)。</span><span class="sxs-lookup"><span data-stu-id="17a11-106">Deletes a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17a11-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="17a11-107">Prerequisites</span></span>
<span data-ttu-id="17a11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17a11-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="17a11-110">Permission type</span></span>|<span data-ttu-id="17a11-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="17a11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17a11-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17a11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17a11-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a11-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17a11-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17a11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17a11-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="17a11-115">Not supported.</span></span>|
|<span data-ttu-id="17a11-116">Application</span><span class="sxs-lookup"><span data-stu-id="17a11-116">Application</span></span>|<span data-ttu-id="17a11-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a11-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17a11-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17a11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="17a11-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="17a11-119">Request headers</span></span>
|<span data-ttu-id="17a11-120">标头</span><span class="sxs-lookup"><span data-stu-id="17a11-120">Header</span></span>|<span data-ttu-id="17a11-121">值</span><span class="sxs-lookup"><span data-stu-id="17a11-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17a11-122">授权</span><span class="sxs-lookup"><span data-stu-id="17a11-122">Authorization</span></span>|<span data-ttu-id="17a11-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="17a11-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17a11-124">接受</span><span class="sxs-lookup"><span data-stu-id="17a11-124">Accept</span></span>|<span data-ttu-id="17a11-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17a11-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17a11-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="17a11-126">Request body</span></span>
<span data-ttu-id="17a11-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17a11-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17a11-128">响应</span><span class="sxs-lookup"><span data-stu-id="17a11-128">Response</span></span>
<span data-ttu-id="17a11-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="17a11-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="17a11-130">示例</span><span class="sxs-lookup"><span data-stu-id="17a11-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="17a11-131">请求</span><span class="sxs-lookup"><span data-stu-id="17a11-131">Request</span></span>
<span data-ttu-id="17a11-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17a11-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="17a11-133">响应</span><span class="sxs-lookup"><span data-stu-id="17a11-133">Response</span></span>
<span data-ttu-id="17a11-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17a11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





