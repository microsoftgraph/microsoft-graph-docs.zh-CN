---
title: getCachedReport 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf2b229601bb7126b7e29f9036f032a4d28b88e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459149"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="dcccc-103">getCachedReport 操作</span><span class="sxs-lookup"><span data-stu-id="dcccc-103">getCachedReport action</span></span>

<span data-ttu-id="dcccc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dcccc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcccc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dcccc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcccc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcccc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcccc-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcccc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dcccc-108">Prerequisites</span></span>
<span data-ttu-id="dcccc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcccc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcccc-111">Permission type</span></span>|<span data-ttu-id="dcccc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dcccc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcccc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcccc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcccc-114">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、Devicemanagementmanageddevices.readwrite.all、all、、all、Devicemanagementmanageddevices.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="dcccc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="dcccc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcccc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcccc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcccc-116">Not supported.</span></span>|
|<span data-ttu-id="dcccc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcccc-117">Application</span></span>|<span data-ttu-id="dcccc-118">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、Devicemanagementmanageddevices.readwrite.all、all、、all、Devicemanagementmanageddevices.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="dcccc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcccc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcccc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="dcccc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcccc-120">Request headers</span></span>
|<span data-ttu-id="dcccc-121">标头</span><span class="sxs-lookup"><span data-stu-id="dcccc-121">Header</span></span>|<span data-ttu-id="dcccc-122">值</span><span class="sxs-lookup"><span data-stu-id="dcccc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcccc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcccc-123">Authorization</span></span>|<span data-ttu-id="dcccc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dcccc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcccc-125">接受</span><span class="sxs-lookup"><span data-stu-id="dcccc-125">Accept</span></span>|<span data-ttu-id="dcccc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcccc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcccc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcccc-127">Request body</span></span>
<span data-ttu-id="dcccc-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcccc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dcccc-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="dcccc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dcccc-130">属性</span><span class="sxs-lookup"><span data-stu-id="dcccc-130">Property</span></span>|<span data-ttu-id="dcccc-131">类型</span><span class="sxs-lookup"><span data-stu-id="dcccc-131">Type</span></span>|<span data-ttu-id="dcccc-132">说明</span><span class="sxs-lookup"><span data-stu-id="dcccc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcccc-133">id</span><span class="sxs-lookup"><span data-stu-id="dcccc-133">id</span></span>|<span data-ttu-id="dcccc-134">String</span><span class="sxs-lookup"><span data-stu-id="dcccc-134">String</span></span>|<span data-ttu-id="dcccc-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-135">Not yet documented</span></span>|
|<span data-ttu-id="dcccc-136">select</span><span class="sxs-lookup"><span data-stu-id="dcccc-136">select</span></span>|<span data-ttu-id="dcccc-137">String collection</span><span class="sxs-lookup"><span data-stu-id="dcccc-137">String collection</span></span>|<span data-ttu-id="dcccc-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-138">Not yet documented</span></span>|
|<span data-ttu-id="dcccc-139">search</span><span class="sxs-lookup"><span data-stu-id="dcccc-139">search</span></span>|<span data-ttu-id="dcccc-140">String</span><span class="sxs-lookup"><span data-stu-id="dcccc-140">String</span></span>|<span data-ttu-id="dcccc-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-141">Not yet documented</span></span>|
|<span data-ttu-id="dcccc-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="dcccc-142">groupBy</span></span>|<span data-ttu-id="dcccc-143">String collection</span><span class="sxs-lookup"><span data-stu-id="dcccc-143">String collection</span></span>|<span data-ttu-id="dcccc-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-144">Not yet documented</span></span>|
|<span data-ttu-id="dcccc-145">By</span><span class="sxs-lookup"><span data-stu-id="dcccc-145">orderBy</span></span>|<span data-ttu-id="dcccc-146">String collection</span><span class="sxs-lookup"><span data-stu-id="dcccc-146">String collection</span></span>|<span data-ttu-id="dcccc-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-147">Not yet documented</span></span>|
|<span data-ttu-id="dcccc-148">skip</span><span class="sxs-lookup"><span data-stu-id="dcccc-148">skip</span></span>|<span data-ttu-id="dcccc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="dcccc-149">Int32</span></span>|<span data-ttu-id="dcccc-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-150">Not yet documented</span></span>|
|<span data-ttu-id="dcccc-151">top</span><span class="sxs-lookup"><span data-stu-id="dcccc-151">top</span></span>|<span data-ttu-id="dcccc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="dcccc-152">Int32</span></span>|<span data-ttu-id="dcccc-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dcccc-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dcccc-154">响应</span><span class="sxs-lookup"><span data-stu-id="dcccc-154">Response</span></span>
<span data-ttu-id="dcccc-155">如果成功，此操作会在`200 OK`响应正文中返回响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="dcccc-155">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcccc-156">示例</span><span class="sxs-lookup"><span data-stu-id="dcccc-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcccc-157">请求</span><span class="sxs-lookup"><span data-stu-id="dcccc-157">Request</span></span>
<span data-ttu-id="dcccc-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcccc-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dcccc-159">响应</span><span class="sxs-lookup"><span data-stu-id="dcccc-159">Response</span></span>
<span data-ttu-id="dcccc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dcccc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```





