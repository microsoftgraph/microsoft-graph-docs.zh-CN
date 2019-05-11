---
title: 删除 sideLoadingKey
description: 删除 sideLoadingKey。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acf93ab6fb2d1dae485c3dc3823c04efed8da467
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899919"
---
# <a name="delete-sideloadingkey"></a><span data-ttu-id="ddceb-103">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="ddceb-103">Delete sideLoadingKey</span></span>

> <span data-ttu-id="ddceb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ddceb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddceb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddceb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddceb-106">删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="ddceb-106">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddceb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddceb-107">Prerequisites</span></span>
<span data-ttu-id="ddceb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddceb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddceb-110">Permission type</span></span>|<span data-ttu-id="ddceb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddceb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddceb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddceb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddceb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddceb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ddceb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddceb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddceb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddceb-115">Not supported.</span></span>|
|<span data-ttu-id="ddceb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddceb-116">Application</span></span>|<span data-ttu-id="ddceb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddceb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddceb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddceb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="ddceb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddceb-119">Request headers</span></span>
|<span data-ttu-id="ddceb-120">标头</span><span class="sxs-lookup"><span data-stu-id="ddceb-120">Header</span></span>|<span data-ttu-id="ddceb-121">值</span><span class="sxs-lookup"><span data-stu-id="ddceb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddceb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddceb-122">Authorization</span></span>|<span data-ttu-id="ddceb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddceb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddceb-124">接受</span><span class="sxs-lookup"><span data-stu-id="ddceb-124">Accept</span></span>|<span data-ttu-id="ddceb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddceb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddceb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddceb-126">Request body</span></span>
<span data-ttu-id="ddceb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddceb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddceb-128">响应</span><span class="sxs-lookup"><span data-stu-id="ddceb-128">Response</span></span>
<span data-ttu-id="ddceb-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ddceb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ddceb-130">示例</span><span class="sxs-lookup"><span data-stu-id="ddceb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddceb-131">请求</span><span class="sxs-lookup"><span data-stu-id="ddceb-131">Request</span></span>
<span data-ttu-id="ddceb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddceb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

### <a name="response"></a><span data-ttu-id="ddceb-133">响应</span><span class="sxs-lookup"><span data-stu-id="ddceb-133">Response</span></span>
<span data-ttu-id="ddceb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddceb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




