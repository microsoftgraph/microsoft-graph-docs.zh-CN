---
title: 删除 androidLobApp
description: 删除 androidLobApp。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbd110d552c8e74819f22fbd677d059ca098336a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700736"
---
# <a name="delete-androidlobapp"></a><span data-ttu-id="81be7-103">删除 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="81be7-103">Delete androidLobApp</span></span>

<span data-ttu-id="81be7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81be7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81be7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81be7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81be7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81be7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81be7-107">删除 [androidLobApp](../resources/intune-apps-androidlobapp.md)。</span><span class="sxs-lookup"><span data-stu-id="81be7-107">Deletes a [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81be7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="81be7-108">Prerequisites</span></span>
<span data-ttu-id="81be7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81be7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81be7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="81be7-111">Permission type</span></span>|<span data-ttu-id="81be7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="81be7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81be7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81be7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81be7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81be7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81be7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81be7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81be7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="81be7-116">Not supported.</span></span>|
|<span data-ttu-id="81be7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="81be7-117">Application</span></span>|<span data-ttu-id="81be7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81be7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81be7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81be7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="81be7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="81be7-120">Request headers</span></span>
|<span data-ttu-id="81be7-121">标头</span><span class="sxs-lookup"><span data-stu-id="81be7-121">Header</span></span>|<span data-ttu-id="81be7-122">值</span><span class="sxs-lookup"><span data-stu-id="81be7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81be7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81be7-123">Authorization</span></span>|<span data-ttu-id="81be7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="81be7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81be7-125">接受</span><span class="sxs-lookup"><span data-stu-id="81be7-125">Accept</span></span>|<span data-ttu-id="81be7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81be7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81be7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="81be7-127">Request body</span></span>
<span data-ttu-id="81be7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81be7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81be7-129">响应</span><span class="sxs-lookup"><span data-stu-id="81be7-129">Response</span></span>
<span data-ttu-id="81be7-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="81be7-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="81be7-131">示例</span><span class="sxs-lookup"><span data-stu-id="81be7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="81be7-132">请求</span><span class="sxs-lookup"><span data-stu-id="81be7-132">Request</span></span>
<span data-ttu-id="81be7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81be7-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="81be7-134">响应</span><span class="sxs-lookup"><span data-stu-id="81be7-134">Response</span></span>
<span data-ttu-id="81be7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="81be7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





