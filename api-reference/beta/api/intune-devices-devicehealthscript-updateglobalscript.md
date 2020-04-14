---
title: updateGlobalScript 操作
description: 更新专用设备运行状况脚本
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42cd16873e374dfbc301674c2a7c76527311581a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426346"
---
# <a name="updateglobalscript-action"></a><span data-ttu-id="6c47e-103">updateGlobalScript 操作</span><span class="sxs-lookup"><span data-stu-id="6c47e-103">updateGlobalScript action</span></span>

<span data-ttu-id="6c47e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c47e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c47e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c47e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c47e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c47e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c47e-107">更新专用设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="6c47e-107">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c47e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c47e-108">Prerequisites</span></span>
<span data-ttu-id="6c47e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c47e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c47e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c47e-111">Permission type</span></span>|<span data-ttu-id="6c47e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c47e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c47e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c47e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c47e-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c47e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c47e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c47e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c47e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c47e-116">Not supported.</span></span>|
|<span data-ttu-id="6c47e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c47e-117">Application</span></span>|<span data-ttu-id="6c47e-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c47e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c47e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c47e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript
```

## <a name="request-headers"></a><span data-ttu-id="6c47e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c47e-120">Request headers</span></span>
|<span data-ttu-id="6c47e-121">标头</span><span class="sxs-lookup"><span data-stu-id="6c47e-121">Header</span></span>|<span data-ttu-id="6c47e-122">值</span><span class="sxs-lookup"><span data-stu-id="6c47e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c47e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c47e-123">Authorization</span></span>|<span data-ttu-id="6c47e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c47e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c47e-125">接受</span><span class="sxs-lookup"><span data-stu-id="6c47e-125">Accept</span></span>|<span data-ttu-id="6c47e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c47e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c47e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c47e-127">Request body</span></span>
<span data-ttu-id="6c47e-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c47e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6c47e-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6c47e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6c47e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6c47e-130">Property</span></span>|<span data-ttu-id="6c47e-131">类型</span><span class="sxs-lookup"><span data-stu-id="6c47e-131">Type</span></span>|<span data-ttu-id="6c47e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6c47e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c47e-133">version</span><span class="sxs-lookup"><span data-stu-id="6c47e-133">version</span></span>|<span data-ttu-id="6c47e-134">String</span><span class="sxs-lookup"><span data-stu-id="6c47e-134">String</span></span>|<span data-ttu-id="6c47e-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6c47e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6c47e-136">响应</span><span class="sxs-lookup"><span data-stu-id="6c47e-136">Response</span></span>
<span data-ttu-id="6c47e-137">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="6c47e-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c47e-138">示例</span><span class="sxs-lookup"><span data-stu-id="6c47e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c47e-139">请求</span><span class="sxs-lookup"><span data-stu-id="6c47e-139">Request</span></span>
<span data-ttu-id="6c47e-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c47e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript

Content-type: application/json
Content-length: 34

{
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="6c47e-141">响应</span><span class="sxs-lookup"><span data-stu-id="6c47e-141">Response</span></span>
<span data-ttu-id="6c47e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c47e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Update Global Script value"
}
```



