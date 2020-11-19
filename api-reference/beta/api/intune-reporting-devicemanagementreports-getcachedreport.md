---
title: getCachedReport 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 920a8171b9d1739d68367179798c00406d62812d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210450"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="f7299-103">getCachedReport 操作</span><span class="sxs-lookup"><span data-stu-id="f7299-103">getCachedReport action</span></span>

<span data-ttu-id="f7299-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7299-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7299-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7299-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7299-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7299-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7299-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7299-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7299-108">Prerequisites</span></span>
<span data-ttu-id="f7299-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7299-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7299-111">Permission type</span></span>|<span data-ttu-id="f7299-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7299-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7299-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7299-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7299-114">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="f7299-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f7299-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7299-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7299-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7299-116">Not supported.</span></span>|
|<span data-ttu-id="f7299-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7299-117">Application</span></span>|<span data-ttu-id="f7299-118">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="f7299-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7299-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7299-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="f7299-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7299-120">Request headers</span></span>
|<span data-ttu-id="f7299-121">标头</span><span class="sxs-lookup"><span data-stu-id="f7299-121">Header</span></span>|<span data-ttu-id="f7299-122">值</span><span class="sxs-lookup"><span data-stu-id="f7299-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7299-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7299-123">Authorization</span></span>|<span data-ttu-id="f7299-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7299-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7299-125">接受</span><span class="sxs-lookup"><span data-stu-id="f7299-125">Accept</span></span>|<span data-ttu-id="f7299-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7299-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7299-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7299-127">Request body</span></span>
<span data-ttu-id="f7299-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7299-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f7299-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f7299-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f7299-130">属性</span><span class="sxs-lookup"><span data-stu-id="f7299-130">Property</span></span>|<span data-ttu-id="f7299-131">类型</span><span class="sxs-lookup"><span data-stu-id="f7299-131">Type</span></span>|<span data-ttu-id="f7299-132">说明</span><span class="sxs-lookup"><span data-stu-id="f7299-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7299-133">id</span><span class="sxs-lookup"><span data-stu-id="f7299-133">id</span></span>|<span data-ttu-id="f7299-134">String</span><span class="sxs-lookup"><span data-stu-id="f7299-134">String</span></span>|<span data-ttu-id="f7299-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-135">Not yet documented</span></span>|
|<span data-ttu-id="f7299-136">select</span><span class="sxs-lookup"><span data-stu-id="f7299-136">select</span></span>|<span data-ttu-id="f7299-137">String collection</span><span class="sxs-lookup"><span data-stu-id="f7299-137">String collection</span></span>|<span data-ttu-id="f7299-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-138">Not yet documented</span></span>|
|<span data-ttu-id="f7299-139">search</span><span class="sxs-lookup"><span data-stu-id="f7299-139">search</span></span>|<span data-ttu-id="f7299-140">String</span><span class="sxs-lookup"><span data-stu-id="f7299-140">String</span></span>|<span data-ttu-id="f7299-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-141">Not yet documented</span></span>|
|<span data-ttu-id="f7299-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="f7299-142">groupBy</span></span>|<span data-ttu-id="f7299-143">String collection</span><span class="sxs-lookup"><span data-stu-id="f7299-143">String collection</span></span>|<span data-ttu-id="f7299-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-144">Not yet documented</span></span>|
|<span data-ttu-id="f7299-145">By</span><span class="sxs-lookup"><span data-stu-id="f7299-145">orderBy</span></span>|<span data-ttu-id="f7299-146">String collection</span><span class="sxs-lookup"><span data-stu-id="f7299-146">String collection</span></span>|<span data-ttu-id="f7299-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-147">Not yet documented</span></span>|
|<span data-ttu-id="f7299-148">skip</span><span class="sxs-lookup"><span data-stu-id="f7299-148">skip</span></span>|<span data-ttu-id="f7299-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f7299-149">Int32</span></span>|<span data-ttu-id="f7299-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-150">Not yet documented</span></span>|
|<span data-ttu-id="f7299-151">top</span><span class="sxs-lookup"><span data-stu-id="f7299-151">top</span></span>|<span data-ttu-id="f7299-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f7299-152">Int32</span></span>|<span data-ttu-id="f7299-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f7299-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7299-154">响应</span><span class="sxs-lookup"><span data-stu-id="f7299-154">Response</span></span>
<span data-ttu-id="f7299-155">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="f7299-155">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7299-156">示例</span><span class="sxs-lookup"><span data-stu-id="f7299-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7299-157">请求</span><span class="sxs-lookup"><span data-stu-id="f7299-157">Request</span></span>
<span data-ttu-id="f7299-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7299-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7299-159">响应</span><span class="sxs-lookup"><span data-stu-id="f7299-159">Response</span></span>
<span data-ttu-id="f7299-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7299-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0Q2FjaGVkUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDc5MjIxODQ3OA=="
}
```




