---
title: approveApps 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 65f7dc0ddb331af74498c3b14c2b276c77399313
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39927501"
---
# <a name="approveapps-action"></a><span data-ttu-id="a2349-103">approveApps 操作</span><span class="sxs-lookup"><span data-stu-id="a2349-103">approveApps action</span></span>

> <span data-ttu-id="a2349-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2349-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2349-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2349-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2349-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a2349-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2349-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2349-107">Prerequisites</span></span>
<span data-ttu-id="a2349-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2349-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2349-110">Permission type</span></span>|<span data-ttu-id="a2349-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2349-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2349-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2349-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2349-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2349-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2349-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2349-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2349-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2349-115">Not supported.</span></span>|
|<span data-ttu-id="a2349-116">Application</span><span class="sxs-lookup"><span data-stu-id="a2349-116">Application</span></span>|<span data-ttu-id="a2349-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2349-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2349-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2349-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps
```

## <a name="request-headers"></a><span data-ttu-id="a2349-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2349-119">Request headers</span></span>
|<span data-ttu-id="a2349-120">标头</span><span class="sxs-lookup"><span data-stu-id="a2349-120">Header</span></span>|<span data-ttu-id="a2349-121">值</span><span class="sxs-lookup"><span data-stu-id="a2349-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2349-122">授权</span><span class="sxs-lookup"><span data-stu-id="a2349-122">Authorization</span></span>|<span data-ttu-id="a2349-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2349-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2349-124">接受</span><span class="sxs-lookup"><span data-stu-id="a2349-124">Accept</span></span>|<span data-ttu-id="a2349-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2349-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2349-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2349-126">Request body</span></span>
<span data-ttu-id="a2349-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2349-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a2349-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a2349-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a2349-129">属性</span><span class="sxs-lookup"><span data-stu-id="a2349-129">Property</span></span>|<span data-ttu-id="a2349-130">类型</span><span class="sxs-lookup"><span data-stu-id="a2349-130">Type</span></span>|<span data-ttu-id="a2349-131">说明</span><span class="sxs-lookup"><span data-stu-id="a2349-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2349-132">packageIds</span><span class="sxs-lookup"><span data-stu-id="a2349-132">packageIds</span></span>|<span data-ttu-id="a2349-133">String collection</span><span class="sxs-lookup"><span data-stu-id="a2349-133">String collection</span></span>|<span data-ttu-id="a2349-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a2349-134">Not yet documented</span></span>|
|<span data-ttu-id="a2349-135">approveAllPermissions</span><span class="sxs-lookup"><span data-stu-id="a2349-135">approveAllPermissions</span></span>|<span data-ttu-id="a2349-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2349-136">Boolean</span></span>|<span data-ttu-id="a2349-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a2349-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a2349-138">响应</span><span class="sxs-lookup"><span data-stu-id="a2349-138">Response</span></span>
<span data-ttu-id="a2349-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a2349-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a2349-140">示例</span><span class="sxs-lookup"><span data-stu-id="a2349-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2349-141">请求</span><span class="sxs-lookup"><span data-stu-id="a2349-141">Request</span></span>
<span data-ttu-id="a2349-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2349-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps

Content-type: application/json
Content-length: 87

{
  "packageIds": [
    "Package Ids value"
  ],
  "approveAllPermissions": true
}
```

### <a name="response"></a><span data-ttu-id="a2349-143">响应</span><span class="sxs-lookup"><span data-stu-id="a2349-143">Response</span></span>
<span data-ttu-id="a2349-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2349-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





