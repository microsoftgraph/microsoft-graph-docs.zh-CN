---
title: 删除 deviceCategory
description: 删除 deviceCategory。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cff7aa7b7c290b37358cef413a0b17e54e91c83c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527166"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="632ca-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="632ca-103">Delete deviceCategory</span></span>

> <span data-ttu-id="632ca-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="632ca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="632ca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="632ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="632ca-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="632ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="632ca-107">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="632ca-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="632ca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="632ca-108">Prerequisites</span></span>
<span data-ttu-id="632ca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="632ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="632ca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="632ca-111">Permission type</span></span>|<span data-ttu-id="632ca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="632ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="632ca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="632ca-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="632ca-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="632ca-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="632ca-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="632ca-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="632ca-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="632ca-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="632ca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="632ca-117">Not supported.</span></span>|
|<span data-ttu-id="632ca-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="632ca-118">Application</span></span>|<span data-ttu-id="632ca-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="632ca-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="632ca-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="632ca-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="632ca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="632ca-121">Request headers</span></span>
|<span data-ttu-id="632ca-122">标头</span><span class="sxs-lookup"><span data-stu-id="632ca-122">Header</span></span>|<span data-ttu-id="632ca-123">值</span><span class="sxs-lookup"><span data-stu-id="632ca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="632ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="632ca-124">Authorization</span></span>|<span data-ttu-id="632ca-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="632ca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="632ca-126">接受</span><span class="sxs-lookup"><span data-stu-id="632ca-126">Accept</span></span>|<span data-ttu-id="632ca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="632ca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="632ca-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="632ca-128">Request body</span></span>
<span data-ttu-id="632ca-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="632ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="632ca-130">响应</span><span class="sxs-lookup"><span data-stu-id="632ca-130">Response</span></span>
<span data-ttu-id="632ca-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="632ca-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="632ca-132">示例</span><span class="sxs-lookup"><span data-stu-id="632ca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="632ca-133">请求</span><span class="sxs-lookup"><span data-stu-id="632ca-133">Request</span></span>

<span data-ttu-id="632ca-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="632ca-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="632ca-135">响应</span><span class="sxs-lookup"><span data-stu-id="632ca-135">Response</span></span>

<span data-ttu-id="632ca-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="632ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



