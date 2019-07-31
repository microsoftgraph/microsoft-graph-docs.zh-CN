---
title: completeSignup 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc85e6bf4d68688b890ca1a3821baf8dc07d8f2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952728"
---
# <a name="completesignup-action"></a><span data-ttu-id="a0e68-103">completeSignup 操作</span><span class="sxs-lookup"><span data-stu-id="a0e68-103">completeSignup action</span></span>

> <span data-ttu-id="a0e68-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0e68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0e68-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0e68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0e68-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a0e68-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0e68-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0e68-107">Prerequisites</span></span>
<span data-ttu-id="a0e68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0e68-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0e68-110">Permission type</span></span>|<span data-ttu-id="a0e68-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a0e68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0e68-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0e68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0e68-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e68-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0e68-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0e68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0e68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0e68-115">Not supported.</span></span>|
|<span data-ttu-id="a0e68-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0e68-116">Application</span></span>|<span data-ttu-id="a0e68-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0e68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0e68-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0e68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="a0e68-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0e68-119">Request headers</span></span>
|<span data-ttu-id="a0e68-120">标头</span><span class="sxs-lookup"><span data-stu-id="a0e68-120">Header</span></span>|<span data-ttu-id="a0e68-121">值</span><span class="sxs-lookup"><span data-stu-id="a0e68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0e68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0e68-122">Authorization</span></span>|<span data-ttu-id="a0e68-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0e68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0e68-124">接受</span><span class="sxs-lookup"><span data-stu-id="a0e68-124">Accept</span></span>|<span data-ttu-id="a0e68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0e68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0e68-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0e68-126">Request body</span></span>
<span data-ttu-id="a0e68-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0e68-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a0e68-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a0e68-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a0e68-129">属性</span><span class="sxs-lookup"><span data-stu-id="a0e68-129">Property</span></span>|<span data-ttu-id="a0e68-130">类型</span><span class="sxs-lookup"><span data-stu-id="a0e68-130">Type</span></span>|<span data-ttu-id="a0e68-131">说明</span><span class="sxs-lookup"><span data-stu-id="a0e68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e68-132">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="a0e68-132">enterpriseToken</span></span>|<span data-ttu-id="a0e68-133">String</span><span class="sxs-lookup"><span data-stu-id="a0e68-133">String</span></span>|<span data-ttu-id="a0e68-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a0e68-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a0e68-135">响应</span><span class="sxs-lookup"><span data-stu-id="a0e68-135">Response</span></span>
<span data-ttu-id="a0e68-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a0e68-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a0e68-137">示例</span><span class="sxs-lookup"><span data-stu-id="a0e68-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0e68-138">请求</span><span class="sxs-lookup"><span data-stu-id="a0e68-138">Request</span></span>
<span data-ttu-id="a0e68-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0e68-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="a0e68-140">响应</span><span class="sxs-lookup"><span data-stu-id="a0e68-140">Response</span></span>
<span data-ttu-id="a0e68-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0e68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





