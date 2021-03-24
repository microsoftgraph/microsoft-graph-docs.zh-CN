---
title: requestSignupUrl 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5aef24c7339401c92686f819dc13433e2ee6228c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141188"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="bf001-103">requestSignupUrl 操作</span><span class="sxs-lookup"><span data-stu-id="bf001-103">requestSignupUrl action</span></span>

<span data-ttu-id="bf001-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf001-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf001-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf001-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf001-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf001-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf001-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf001-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf001-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf001-108">Prerequisites</span></span>
<span data-ttu-id="bf001-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf001-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf001-111">Permission type</span></span>|<span data-ttu-id="bf001-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf001-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf001-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf001-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf001-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf001-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf001-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf001-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf001-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf001-116">Not supported.</span></span>|
|<span data-ttu-id="bf001-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf001-117">Application</span></span>|<span data-ttu-id="bf001-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf001-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf001-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf001-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="bf001-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf001-120">Request headers</span></span>
|<span data-ttu-id="bf001-121">标头</span><span class="sxs-lookup"><span data-stu-id="bf001-121">Header</span></span>|<span data-ttu-id="bf001-122">值</span><span class="sxs-lookup"><span data-stu-id="bf001-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf001-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf001-123">Authorization</span></span>|<span data-ttu-id="bf001-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf001-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf001-125">接受</span><span class="sxs-lookup"><span data-stu-id="bf001-125">Accept</span></span>|<span data-ttu-id="bf001-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf001-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf001-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf001-127">Request body</span></span>
<span data-ttu-id="bf001-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf001-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bf001-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="bf001-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bf001-130">属性</span><span class="sxs-lookup"><span data-stu-id="bf001-130">Property</span></span>|<span data-ttu-id="bf001-131">类型</span><span class="sxs-lookup"><span data-stu-id="bf001-131">Type</span></span>|<span data-ttu-id="bf001-132">说明</span><span class="sxs-lookup"><span data-stu-id="bf001-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf001-133">hostName</span><span class="sxs-lookup"><span data-stu-id="bf001-133">hostName</span></span>|<span data-ttu-id="bf001-134">String</span><span class="sxs-lookup"><span data-stu-id="bf001-134">String</span></span>|<span data-ttu-id="bf001-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf001-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bf001-136">响应</span><span class="sxs-lookup"><span data-stu-id="bf001-136">Response</span></span>
<span data-ttu-id="bf001-137">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="bf001-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf001-138">示例</span><span class="sxs-lookup"><span data-stu-id="bf001-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf001-139">请求</span><span class="sxs-lookup"><span data-stu-id="bf001-139">Request</span></span>
<span data-ttu-id="bf001-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf001-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="bf001-141">响应</span><span class="sxs-lookup"><span data-stu-id="bf001-141">Response</span></span>
<span data-ttu-id="bf001-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf001-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```




