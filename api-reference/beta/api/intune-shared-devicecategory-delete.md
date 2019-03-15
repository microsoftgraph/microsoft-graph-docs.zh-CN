---
title: 删除 deviceCategory
description: 删除 deviceCategory。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef1283329ac40356a4f81704b1969aebbb8b0dde
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571128"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="8d2b4-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8d2b4-103">Delete deviceCategory</span></span>

> <span data-ttu-id="8d2b4-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d2b4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d2b4-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d2b4-107">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d2b4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d2b4-108">Prerequisites</span></span>
<span data-ttu-id="8d2b4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8d2b4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d2b4-111">Permission type</span></span>|<span data-ttu-id="8d2b4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8d2b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d2b4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d2b4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8d2b4-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="8d2b4-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8d2b4-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d2b4-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8d2b4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d2b4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d2b4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-117">Not supported.</span></span>|
|<span data-ttu-id="8d2b4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d2b4-118">Application</span></span>|<span data-ttu-id="8d2b4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d2b4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d2b4-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="8d2b4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d2b4-121">Request headers</span></span>
|<span data-ttu-id="8d2b4-122">标头</span><span class="sxs-lookup"><span data-stu-id="8d2b4-122">Header</span></span>|<span data-ttu-id="8d2b4-123">值</span><span class="sxs-lookup"><span data-stu-id="8d2b4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d2b4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d2b4-124">Authorization</span></span>|<span data-ttu-id="8d2b4-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d2b4-126">接受</span><span class="sxs-lookup"><span data-stu-id="8d2b4-126">Accept</span></span>|<span data-ttu-id="8d2b4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8d2b4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d2b4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d2b4-128">Request body</span></span>
<span data-ttu-id="8d2b4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d2b4-130">响应</span><span class="sxs-lookup"><span data-stu-id="8d2b4-130">Response</span></span>
<span data-ttu-id="8d2b4-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d2b4-132">示例</span><span class="sxs-lookup"><span data-stu-id="8d2b4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d2b4-133">请求</span><span class="sxs-lookup"><span data-stu-id="8d2b4-133">Request</span></span>

<span data-ttu-id="8d2b4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="8d2b4-135">响应</span><span class="sxs-lookup"><span data-stu-id="8d2b4-135">Response</span></span>

<span data-ttu-id="8d2b4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d2b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



