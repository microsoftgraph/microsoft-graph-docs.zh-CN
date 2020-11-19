---
title: getGlobalScriptHighestAvailableVersion 操作
description: 更新专用设备运行状况脚本
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7d043f9f75e78ad56b3c2f98cae385c0540179a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49264084"
---
# <a name="getglobalscripthighestavailableversion-action"></a><span data-ttu-id="f27d6-103">getGlobalScriptHighestAvailableVersion 操作</span><span class="sxs-lookup"><span data-stu-id="f27d6-103">getGlobalScriptHighestAvailableVersion action</span></span>

<span data-ttu-id="f27d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f27d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f27d6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f27d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f27d6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f27d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f27d6-107">更新专用设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="f27d6-107">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f27d6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f27d6-108">Prerequisites</span></span>
<span data-ttu-id="f27d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f27d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f27d6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f27d6-111">Permission type</span></span>|<span data-ttu-id="f27d6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f27d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f27d6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f27d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f27d6-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f27d6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f27d6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f27d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f27d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f27d6-116">Not supported.</span></span>|
|<span data-ttu-id="f27d6-117">Application</span><span class="sxs-lookup"><span data-stu-id="f27d6-117">Application</span></span>|<span data-ttu-id="f27d6-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f27d6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f27d6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f27d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

## <a name="request-headers"></a><span data-ttu-id="f27d6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f27d6-120">Request headers</span></span>
|<span data-ttu-id="f27d6-121">标头</span><span class="sxs-lookup"><span data-stu-id="f27d6-121">Header</span></span>|<span data-ttu-id="f27d6-122">值</span><span class="sxs-lookup"><span data-stu-id="f27d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f27d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f27d6-123">Authorization</span></span>|<span data-ttu-id="f27d6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f27d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f27d6-125">接受</span><span class="sxs-lookup"><span data-stu-id="f27d6-125">Accept</span></span>|<span data-ttu-id="f27d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f27d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f27d6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f27d6-127">Request body</span></span>
<span data-ttu-id="f27d6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f27d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f27d6-129">响应</span><span class="sxs-lookup"><span data-stu-id="f27d6-129">Response</span></span>
<span data-ttu-id="f27d6-130">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="f27d6-130">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f27d6-131">示例</span><span class="sxs-lookup"><span data-stu-id="f27d6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f27d6-132">请求</span><span class="sxs-lookup"><span data-stu-id="f27d6-132">Request</span></span>
<span data-ttu-id="f27d6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f27d6-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

### <a name="response"></a><span data-ttu-id="f27d6-134">响应</span><span class="sxs-lookup"><span data-stu-id="f27d6-134">Response</span></span>
<span data-ttu-id="f27d6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f27d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 68

{
  "value": "Get Global Script Highest Available Version value"
}
```




