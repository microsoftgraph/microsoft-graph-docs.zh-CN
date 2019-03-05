---
title: setPriority 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bca4f7c57efc47ed6a85710a453b354586a736f9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255540"
---
# <a name="setpriority-action"></a><span data-ttu-id="a82a9-103">setPriority 操作</span><span class="sxs-lookup"><span data-stu-id="a82a9-103">setPriority action</span></span>

> <span data-ttu-id="a82a9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a82a9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a82a9-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a82a9-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a82a9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a82a9-106">Prerequisites</span></span>
<span data-ttu-id="a82a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a82a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a82a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a82a9-109">Permission type</span></span>|<span data-ttu-id="a82a9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a82a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a82a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a82a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a82a9-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82a9-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a82a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a82a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a82a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a82a9-114">Not supported.</span></span>|
|<span data-ttu-id="a82a9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a82a9-115">Application</span></span>|<span data-ttu-id="a82a9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a82a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a82a9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a82a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="a82a9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a82a9-118">Request headers</span></span>
|<span data-ttu-id="a82a9-119">标头</span><span class="sxs-lookup"><span data-stu-id="a82a9-119">Header</span></span>|<span data-ttu-id="a82a9-120">值</span><span class="sxs-lookup"><span data-stu-id="a82a9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a82a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a82a9-121">Authorization</span></span>|<span data-ttu-id="a82a9-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a82a9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a82a9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a82a9-123">Accept</span></span>|<span data-ttu-id="a82a9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a82a9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a82a9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a82a9-125">Request body</span></span>
<span data-ttu-id="a82a9-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a82a9-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a82a9-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a82a9-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a82a9-128">属性</span><span class="sxs-lookup"><span data-stu-id="a82a9-128">Property</span></span>|<span data-ttu-id="a82a9-129">类型</span><span class="sxs-lookup"><span data-stu-id="a82a9-129">Type</span></span>|<span data-ttu-id="a82a9-130">说明</span><span class="sxs-lookup"><span data-stu-id="a82a9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a82a9-131">priority</span><span class="sxs-lookup"><span data-stu-id="a82a9-131">priority</span></span>|<span data-ttu-id="a82a9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="a82a9-132">Int32</span></span>|<span data-ttu-id="a82a9-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a82a9-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a82a9-134">响应</span><span class="sxs-lookup"><span data-stu-id="a82a9-134">Response</span></span>
<span data-ttu-id="a82a9-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a82a9-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a82a9-136">示例</span><span class="sxs-lookup"><span data-stu-id="a82a9-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a82a9-137">请求</span><span class="sxs-lookup"><span data-stu-id="a82a9-137">Request</span></span>
<span data-ttu-id="a82a9-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a82a9-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="a82a9-139">响应</span><span class="sxs-lookup"><span data-stu-id="a82a9-139">Response</span></span>
<span data-ttu-id="a82a9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a82a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



