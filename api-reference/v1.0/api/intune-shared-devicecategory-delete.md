---
title: 删除 deviceCategory
description: 删除 deviceCategory。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35dffc1c280caeb10007dbf11d390ac7487d4a61
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249968"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="5baac-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5baac-103">Delete deviceCategory</span></span>

> <span data-ttu-id="5baac-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5baac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5baac-105">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="5baac-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5baac-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5baac-106">Prerequisites</span></span>
<span data-ttu-id="5baac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5baac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5baac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5baac-109">Permission type</span></span>|<span data-ttu-id="5baac-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5baac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5baac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5baac-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5baac-112">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="5baac-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5baac-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5baac-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5baac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5baac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5baac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5baac-115">Not supported.</span></span>|
|<span data-ttu-id="5baac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5baac-116">Application</span></span>|<span data-ttu-id="5baac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5baac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5baac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5baac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5baac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5baac-119">Request headers</span></span>
|<span data-ttu-id="5baac-120">标头</span><span class="sxs-lookup"><span data-stu-id="5baac-120">Header</span></span>|<span data-ttu-id="5baac-121">值</span><span class="sxs-lookup"><span data-stu-id="5baac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5baac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5baac-122">Authorization</span></span>|<span data-ttu-id="5baac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5baac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5baac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5baac-124">Accept</span></span>|<span data-ttu-id="5baac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5baac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5baac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5baac-126">Request body</span></span>
<span data-ttu-id="5baac-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5baac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5baac-128">响应</span><span class="sxs-lookup"><span data-stu-id="5baac-128">Response</span></span>
<span data-ttu-id="5baac-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5baac-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5baac-130">示例</span><span class="sxs-lookup"><span data-stu-id="5baac-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="5baac-131">请求</span><span class="sxs-lookup"><span data-stu-id="5baac-131">Request</span></span>
<span data-ttu-id="5baac-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5baac-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="5baac-133">响应</span><span class="sxs-lookup"><span data-stu-id="5baac-133">Response</span></span>
<span data-ttu-id="5baac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5baac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



