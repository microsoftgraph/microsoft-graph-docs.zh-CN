---
title: getCachedReport 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d64fba30bf2eed48fe14a203c85e0ceab977c4a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537245"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="b76a3-103">getCachedReport 操作</span><span class="sxs-lookup"><span data-stu-id="b76a3-103">getCachedReport action</span></span>

> <span data-ttu-id="b76a3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b76a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b76a3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b76a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b76a3-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b76a3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b76a3-107">Prerequisites</span></span>
<span data-ttu-id="b76a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b76a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b76a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b76a3-110">Permission type</span></span>|<span data-ttu-id="b76a3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b76a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b76a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b76a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b76a3-113">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、Devicemanagementmanageddevices.readwrite.all、all、、all、Devicemanagementmanageddevices.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="b76a3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b76a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b76a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b76a3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b76a3-115">Not supported.</span></span>|
|<span data-ttu-id="b76a3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b76a3-116">Application</span></span>|<span data-ttu-id="b76a3-117">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、Devicemanagementmanageddevices.readwrite.all、all、、all、Devicemanagementmanageddevices.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="b76a3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b76a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b76a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="b76a3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b76a3-119">Request headers</span></span>
|<span data-ttu-id="b76a3-120">标头</span><span class="sxs-lookup"><span data-stu-id="b76a3-120">Header</span></span>|<span data-ttu-id="b76a3-121">值</span><span class="sxs-lookup"><span data-stu-id="b76a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b76a3-122">授权</span><span class="sxs-lookup"><span data-stu-id="b76a3-122">Authorization</span></span>|<span data-ttu-id="b76a3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b76a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b76a3-124">接受</span><span class="sxs-lookup"><span data-stu-id="b76a3-124">Accept</span></span>|<span data-ttu-id="b76a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b76a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b76a3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b76a3-126">Request body</span></span>
<span data-ttu-id="b76a3-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b76a3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b76a3-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b76a3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b76a3-129">属性</span><span class="sxs-lookup"><span data-stu-id="b76a3-129">Property</span></span>|<span data-ttu-id="b76a3-130">类型</span><span class="sxs-lookup"><span data-stu-id="b76a3-130">Type</span></span>|<span data-ttu-id="b76a3-131">说明</span><span class="sxs-lookup"><span data-stu-id="b76a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76a3-132">id</span><span class="sxs-lookup"><span data-stu-id="b76a3-132">id</span></span>|<span data-ttu-id="b76a3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b76a3-133">String</span></span>|<span data-ttu-id="b76a3-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-134">Not yet documented</span></span>|
|<span data-ttu-id="b76a3-135">select</span><span class="sxs-lookup"><span data-stu-id="b76a3-135">select</span></span>|<span data-ttu-id="b76a3-136">String collection</span><span class="sxs-lookup"><span data-stu-id="b76a3-136">String collection</span></span>|<span data-ttu-id="b76a3-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-137">Not yet documented</span></span>|
|<span data-ttu-id="b76a3-138">search</span><span class="sxs-lookup"><span data-stu-id="b76a3-138">search</span></span>|<span data-ttu-id="b76a3-139">String</span><span class="sxs-lookup"><span data-stu-id="b76a3-139">String</span></span>|<span data-ttu-id="b76a3-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-140">Not yet documented</span></span>|
|<span data-ttu-id="b76a3-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="b76a3-141">groupBy</span></span>|<span data-ttu-id="b76a3-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b76a3-142">String collection</span></span>|<span data-ttu-id="b76a3-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-143">Not yet documented</span></span>|
|<span data-ttu-id="b76a3-144">By</span><span class="sxs-lookup"><span data-stu-id="b76a3-144">orderBy</span></span>|<span data-ttu-id="b76a3-145">String collection</span><span class="sxs-lookup"><span data-stu-id="b76a3-145">String collection</span></span>|<span data-ttu-id="b76a3-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-146">Not yet documented</span></span>|
|<span data-ttu-id="b76a3-147">skip</span><span class="sxs-lookup"><span data-stu-id="b76a3-147">skip</span></span>|<span data-ttu-id="b76a3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b76a3-148">Int32</span></span>|<span data-ttu-id="b76a3-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-149">Not yet documented</span></span>|
|<span data-ttu-id="b76a3-150">top</span><span class="sxs-lookup"><span data-stu-id="b76a3-150">top</span></span>|<span data-ttu-id="b76a3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b76a3-151">Int32</span></span>|<span data-ttu-id="b76a3-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b76a3-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b76a3-153">响应</span><span class="sxs-lookup"><span data-stu-id="b76a3-153">Response</span></span>
<span data-ttu-id="b76a3-154">如果成功，此操作会在`200 OK`响应正文中返回响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="b76a3-154">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b76a3-155">示例</span><span class="sxs-lookup"><span data-stu-id="b76a3-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b76a3-156">请求</span><span class="sxs-lookup"><span data-stu-id="b76a3-156">Request</span></span>
<span data-ttu-id="b76a3-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b76a3-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCachedReport

Content-type: application/json
Content-length: 209

{
  "id": "Id value",
  "select": [
    "Select value"
  ],
  "search": "Search value",
  "groupBy": [
    "Group By value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "skip": 4,
  "top": 3
}
```

### <a name="response"></a><span data-ttu-id="b76a3-158">响应</span><span class="sxs-lookup"><span data-stu-id="b76a3-158">Response</span></span>
<span data-ttu-id="b76a3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b76a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```






