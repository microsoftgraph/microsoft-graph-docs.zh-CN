---
title: setPriority 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9a18689ddf05db06e7b6ad390363457305e978e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057379"
---
# <a name="setpriority-action"></a><span data-ttu-id="afefb-103">setPriority 操作</span><span class="sxs-lookup"><span data-stu-id="afefb-103">setPriority action</span></span>

<span data-ttu-id="afefb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afefb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afefb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afefb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afefb-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="afefb-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afefb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="afefb-107">Prerequisites</span></span>
<span data-ttu-id="afefb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afefb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="afefb-110">Permission type</span></span>|<span data-ttu-id="afefb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="afefb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afefb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afefb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afefb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afefb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="afefb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afefb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afefb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="afefb-115">Not supported.</span></span>|
|<span data-ttu-id="afefb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="afefb-116">Application</span></span>|<span data-ttu-id="afefb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="afefb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afefb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afefb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="afefb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="afefb-119">Request headers</span></span>
|<span data-ttu-id="afefb-120">标头</span><span class="sxs-lookup"><span data-stu-id="afefb-120">Header</span></span>|<span data-ttu-id="afefb-121">值</span><span class="sxs-lookup"><span data-stu-id="afefb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afefb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afefb-122">Authorization</span></span>|<span data-ttu-id="afefb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="afefb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afefb-124">接受</span><span class="sxs-lookup"><span data-stu-id="afefb-124">Accept</span></span>|<span data-ttu-id="afefb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afefb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afefb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="afefb-126">Request body</span></span>
<span data-ttu-id="afefb-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afefb-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="afefb-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="afefb-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="afefb-129">属性</span><span class="sxs-lookup"><span data-stu-id="afefb-129">Property</span></span>|<span data-ttu-id="afefb-130">类型</span><span class="sxs-lookup"><span data-stu-id="afefb-130">Type</span></span>|<span data-ttu-id="afefb-131">说明</span><span class="sxs-lookup"><span data-stu-id="afefb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afefb-132">priority</span><span class="sxs-lookup"><span data-stu-id="afefb-132">priority</span></span>|<span data-ttu-id="afefb-133">Int32</span><span class="sxs-lookup"><span data-stu-id="afefb-133">Int32</span></span>|<span data-ttu-id="afefb-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="afefb-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="afefb-135">响应</span><span class="sxs-lookup"><span data-stu-id="afefb-135">Response</span></span>
<span data-ttu-id="afefb-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="afefb-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="afefb-137">示例</span><span class="sxs-lookup"><span data-stu-id="afefb-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="afefb-138">请求</span><span class="sxs-lookup"><span data-stu-id="afefb-138">Request</span></span>
<span data-ttu-id="afefb-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afefb-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="afefb-140">响应</span><span class="sxs-lookup"><span data-stu-id="afefb-140">Response</span></span>
<span data-ttu-id="afefb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afefb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









