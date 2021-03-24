---
title: scopedForResource 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b6ba67c90220c9a5461b1d8b4b40c9e00582045
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148482"
---
# <a name="scopedforresource-function"></a><span data-ttu-id="2f505-103">scopedForResource 函数</span><span class="sxs-lookup"><span data-stu-id="2f505-103">scopedForResource function</span></span>

<span data-ttu-id="2f505-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f505-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f505-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f505-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f505-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f505-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f505-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f505-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f505-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f505-108">Prerequisites</span></span>
<span data-ttu-id="2f505-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f505-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f505-111">Permission type</span></span>|<span data-ttu-id="2f505-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f505-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f505-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f505-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f505-114">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f505-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2f505-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f505-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f505-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f505-116">Not supported.</span></span>|
|<span data-ttu-id="2f505-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f505-117">Application</span></span>|<span data-ttu-id="2f505-118">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f505-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f505-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f505-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/scopedForResource
```

## <a name="request-headers"></a><span data-ttu-id="2f505-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f505-120">Request headers</span></span>
|<span data-ttu-id="2f505-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f505-121">Header</span></span>|<span data-ttu-id="2f505-122">值</span><span class="sxs-lookup"><span data-stu-id="2f505-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f505-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f505-123">Authorization</span></span>|<span data-ttu-id="2f505-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f505-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f505-125">接受</span><span class="sxs-lookup"><span data-stu-id="2f505-125">Accept</span></span>|<span data-ttu-id="2f505-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f505-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f505-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f505-127">Request body</span></span>
<span data-ttu-id="2f505-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="2f505-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2f505-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="2f505-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2f505-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f505-130">Property</span></span>|<span data-ttu-id="2f505-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f505-131">Type</span></span>|<span data-ttu-id="2f505-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f505-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f505-133">资源</span><span class="sxs-lookup"><span data-stu-id="2f505-133">resource</span></span>|<span data-ttu-id="2f505-134">String</span><span class="sxs-lookup"><span data-stu-id="2f505-134">String</span></span>|<span data-ttu-id="2f505-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f505-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2f505-136">响应</span><span class="sxs-lookup"><span data-stu-id="2f505-136">Response</span></span>
<span data-ttu-id="2f505-137">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Boolean。</span><span class="sxs-lookup"><span data-stu-id="2f505-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f505-138">示例</span><span class="sxs-lookup"><span data-stu-id="2f505-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f505-139">请求</span><span class="sxs-lookup"><span data-stu-id="2f505-139">Request</span></span>
<span data-ttu-id="2f505-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f505-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/scopedForResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2f505-141">响应</span><span class="sxs-lookup"><span data-stu-id="2f505-141">Response</span></span>
<span data-ttu-id="2f505-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f505-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




