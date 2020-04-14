---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 362a673ba2fd13d6e82c59c0d18b75a7af6eaa8a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452265"
---
# <a name="assign-action"></a><span data-ttu-id="71d59-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="71d59-103">assign action</span></span>

<span data-ttu-id="71d59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71d59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71d59-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71d59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71d59-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71d59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71d59-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="71d59-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d59-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="71d59-108">Prerequisites</span></span>
<span data-ttu-id="71d59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71d59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71d59-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71d59-111">Permission type</span></span>|<span data-ttu-id="71d59-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71d59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71d59-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71d59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71d59-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d59-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71d59-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71d59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71d59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71d59-116">Not supported.</span></span>|
|<span data-ttu-id="71d59-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="71d59-117">Application</span></span>|<span data-ttu-id="71d59-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d59-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71d59-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71d59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="71d59-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="71d59-120">Request headers</span></span>
|<span data-ttu-id="71d59-121">标头</span><span class="sxs-lookup"><span data-stu-id="71d59-121">Header</span></span>|<span data-ttu-id="71d59-122">值</span><span class="sxs-lookup"><span data-stu-id="71d59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71d59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71d59-123">Authorization</span></span>|<span data-ttu-id="71d59-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71d59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71d59-125">接受</span><span class="sxs-lookup"><span data-stu-id="71d59-125">Accept</span></span>|<span data-ttu-id="71d59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71d59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71d59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="71d59-127">Request body</span></span>
<span data-ttu-id="71d59-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71d59-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="71d59-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="71d59-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="71d59-130">属性</span><span class="sxs-lookup"><span data-stu-id="71d59-130">Property</span></span>|<span data-ttu-id="71d59-131">类型</span><span class="sxs-lookup"><span data-stu-id="71d59-131">Type</span></span>|<span data-ttu-id="71d59-132">说明</span><span class="sxs-lookup"><span data-stu-id="71d59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d59-133">assignments</span><span class="sxs-lookup"><span data-stu-id="71d59-133">assignments</span></span>|<span data-ttu-id="71d59-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="71d59-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="71d59-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="71d59-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="71d59-136">响应</span><span class="sxs-lookup"><span data-stu-id="71d59-136">Response</span></span>
<span data-ttu-id="71d59-137">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合。</span><span class="sxs-lookup"><span data-stu-id="71d59-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d59-138">示例</span><span class="sxs-lookup"><span data-stu-id="71d59-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="71d59-139">请求</span><span class="sxs-lookup"><span data-stu-id="71d59-139">Request</span></span>
<span data-ttu-id="71d59-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71d59-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 287

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="71d59-141">响应</span><span class="sxs-lookup"><span data-stu-id="71d59-141">Response</span></span>
<span data-ttu-id="71d59-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71d59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



