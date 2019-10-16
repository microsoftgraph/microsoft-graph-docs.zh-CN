---
title: 删除 deviceCategory
description: 删除 deviceCategory。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04274c860e56f0d9fe339d9226b1bcb652cd1448
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537097"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="b72fb-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b72fb-103">Delete deviceCategory</span></span>

> <span data-ttu-id="b72fb-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b72fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b72fb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b72fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b72fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b72fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b72fb-107">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="b72fb-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b72fb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b72fb-108">Prerequisites</span></span>
<span data-ttu-id="b72fb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b72fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b72fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b72fb-111">Permission type</span></span>|<span data-ttu-id="b72fb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b72fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b72fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b72fb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b72fb-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="b72fb-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b72fb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b72fb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b72fb-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b72fb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b72fb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b72fb-117">Not supported.</span></span>|
|<span data-ttu-id="b72fb-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b72fb-118">Application</span></span>||
| <span data-ttu-id="b72fb-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="b72fb-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b72fb-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b72fb-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b72fb-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b72fb-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="b72fb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b72fb-122">Request headers</span></span>
|<span data-ttu-id="b72fb-123">标头</span><span class="sxs-lookup"><span data-stu-id="b72fb-123">Header</span></span>|<span data-ttu-id="b72fb-124">值</span><span class="sxs-lookup"><span data-stu-id="b72fb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b72fb-125">授权</span><span class="sxs-lookup"><span data-stu-id="b72fb-125">Authorization</span></span>|<span data-ttu-id="b72fb-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b72fb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b72fb-127">接受</span><span class="sxs-lookup"><span data-stu-id="b72fb-127">Accept</span></span>|<span data-ttu-id="b72fb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b72fb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b72fb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b72fb-129">Request body</span></span>
<span data-ttu-id="b72fb-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b72fb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b72fb-131">响应</span><span class="sxs-lookup"><span data-stu-id="b72fb-131">Response</span></span>
<span data-ttu-id="b72fb-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b72fb-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b72fb-133">示例</span><span class="sxs-lookup"><span data-stu-id="b72fb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b72fb-134">请求</span><span class="sxs-lookup"><span data-stu-id="b72fb-134">Request</span></span>

<span data-ttu-id="b72fb-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b72fb-135">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="b72fb-136">响应</span><span class="sxs-lookup"><span data-stu-id="b72fb-136">Response</span></span>

<span data-ttu-id="b72fb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b72fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









