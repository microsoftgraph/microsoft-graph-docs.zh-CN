---
title: 删除 win32LobApp
description: 删除 win32LobApp。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8c6d5b86f664fdf5b6f493b5dcf1b071899da19
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247305"
---
# <a name="delete-win32lobapp"></a><span data-ttu-id="6fb57-103">删除 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="6fb57-103">Delete win32LobApp</span></span>

<span data-ttu-id="6fb57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fb57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fb57-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6fb57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fb57-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fb57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fb57-107">删除 [win32LobApp](../resources/intune-apps-win32lobapp.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb57-107">Deletes a [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fb57-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6fb57-108">Prerequisites</span></span>
<span data-ttu-id="6fb57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fb57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb57-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fb57-111">Permission type</span></span>|<span data-ttu-id="6fb57-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6fb57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fb57-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fb57-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb57-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6fb57-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fb57-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fb57-116">Not supported.</span></span>|
|<span data-ttu-id="6fb57-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fb57-117">Application</span></span>|<span data-ttu-id="6fb57-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb57-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fb57-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fb57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6fb57-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fb57-120">Request headers</span></span>
|<span data-ttu-id="6fb57-121">标头</span><span class="sxs-lookup"><span data-stu-id="6fb57-121">Header</span></span>|<span data-ttu-id="6fb57-122">值</span><span class="sxs-lookup"><span data-stu-id="6fb57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fb57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fb57-123">Authorization</span></span>|<span data-ttu-id="6fb57-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6fb57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fb57-125">接受</span><span class="sxs-lookup"><span data-stu-id="6fb57-125">Accept</span></span>|<span data-ttu-id="6fb57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fb57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fb57-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fb57-127">Request body</span></span>
<span data-ttu-id="6fb57-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fb57-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb57-129">响应</span><span class="sxs-lookup"><span data-stu-id="6fb57-129">Response</span></span>
<span data-ttu-id="6fb57-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6fb57-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6fb57-131">示例</span><span class="sxs-lookup"><span data-stu-id="6fb57-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fb57-132">请求</span><span class="sxs-lookup"><span data-stu-id="6fb57-132">Request</span></span>
<span data-ttu-id="6fb57-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fb57-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="6fb57-134">响应</span><span class="sxs-lookup"><span data-stu-id="6fb57-134">Response</span></span>
<span data-ttu-id="6fb57-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fb57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




