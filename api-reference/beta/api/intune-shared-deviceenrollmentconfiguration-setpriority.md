---
title: setPriority 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f2645e29c76d427920d558993f6825bff455e95
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390306"
---
# <a name="setpriority-action"></a><span data-ttu-id="4377d-103">setPriority 操作</span><span class="sxs-lookup"><span data-stu-id="4377d-103">setPriority action</span></span>

<span data-ttu-id="4377d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4377d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4377d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4377d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4377d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4377d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4377d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4377d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4377d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4377d-108">Prerequisites</span></span>
<span data-ttu-id="4377d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4377d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4377d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4377d-111">Permission type</span></span>|<span data-ttu-id="4377d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4377d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4377d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4377d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4377d-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4377d-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4377d-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4377d-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4377d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4377d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4377d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4377d-117">Not supported.</span></span>|
|<span data-ttu-id="4377d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4377d-118">Application</span></span>||
| <span data-ttu-id="4377d-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4377d-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4377d-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4377d-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4377d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4377d-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="4377d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4377d-122">Request headers</span></span>
|<span data-ttu-id="4377d-123">标头</span><span class="sxs-lookup"><span data-stu-id="4377d-123">Header</span></span>|<span data-ttu-id="4377d-124">值</span><span class="sxs-lookup"><span data-stu-id="4377d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4377d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4377d-125">Authorization</span></span>|<span data-ttu-id="4377d-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4377d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4377d-127">接受</span><span class="sxs-lookup"><span data-stu-id="4377d-127">Accept</span></span>|<span data-ttu-id="4377d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4377d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4377d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4377d-129">Request body</span></span>
<span data-ttu-id="4377d-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4377d-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4377d-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="4377d-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4377d-132">属性</span><span class="sxs-lookup"><span data-stu-id="4377d-132">Property</span></span>|<span data-ttu-id="4377d-133">类型</span><span class="sxs-lookup"><span data-stu-id="4377d-133">Type</span></span>|<span data-ttu-id="4377d-134">说明</span><span class="sxs-lookup"><span data-stu-id="4377d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4377d-135">priority</span><span class="sxs-lookup"><span data-stu-id="4377d-135">priority</span></span>|<span data-ttu-id="4377d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4377d-136">Int32</span></span>|<span data-ttu-id="4377d-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4377d-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4377d-138">响应</span><span class="sxs-lookup"><span data-stu-id="4377d-138">Response</span></span>
<span data-ttu-id="4377d-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4377d-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4377d-140">示例</span><span class="sxs-lookup"><span data-stu-id="4377d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4377d-141">请求</span><span class="sxs-lookup"><span data-stu-id="4377d-141">Request</span></span>
<span data-ttu-id="4377d-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4377d-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="4377d-143">响应</span><span class="sxs-lookup"><span data-stu-id="4377d-143">Response</span></span>
<span data-ttu-id="4377d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4377d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






