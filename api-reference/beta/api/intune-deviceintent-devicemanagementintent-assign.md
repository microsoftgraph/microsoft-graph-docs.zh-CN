---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00f823751f1c33bae8a0fcde79639efea840b043
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181005"
---
# <a name="assign-action"></a><span data-ttu-id="ca548-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="ca548-103">assign action</span></span>

> <span data-ttu-id="ca548-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca548-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca548-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca548-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca548-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ca548-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca548-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca548-107">Prerequisites</span></span>
<span data-ttu-id="ca548-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca548-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca548-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca548-110">Permission type</span></span>|<span data-ttu-id="ca548-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca548-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca548-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca548-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca548-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca548-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca548-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca548-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca548-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca548-115">Not supported.</span></span>|
|<span data-ttu-id="ca548-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca548-116">Application</span></span>|<span data-ttu-id="ca548-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca548-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca548-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca548-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ca548-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca548-119">Request headers</span></span>
|<span data-ttu-id="ca548-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca548-120">Header</span></span>|<span data-ttu-id="ca548-121">值</span><span class="sxs-lookup"><span data-stu-id="ca548-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca548-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca548-122">Authorization</span></span>|<span data-ttu-id="ca548-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca548-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca548-124">接受</span><span class="sxs-lookup"><span data-stu-id="ca548-124">Accept</span></span>|<span data-ttu-id="ca548-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca548-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca548-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca548-126">Request body</span></span>
<span data-ttu-id="ca548-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca548-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ca548-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ca548-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ca548-129">属性</span><span class="sxs-lookup"><span data-stu-id="ca548-129">Property</span></span>|<span data-ttu-id="ca548-130">类型</span><span class="sxs-lookup"><span data-stu-id="ca548-130">Type</span></span>|<span data-ttu-id="ca548-131">说明</span><span class="sxs-lookup"><span data-stu-id="ca548-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca548-132">assignments</span><span class="sxs-lookup"><span data-stu-id="ca548-132">assignments</span></span>|<span data-ttu-id="ca548-133">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca548-133">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="ca548-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ca548-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ca548-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca548-135">Response</span></span>
<span data-ttu-id="ca548-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ca548-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ca548-137">示例</span><span class="sxs-lookup"><span data-stu-id="ca548-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca548-138">请求</span><span class="sxs-lookup"><span data-stu-id="ca548-138">Request</span></span>
<span data-ttu-id="ca548-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca548-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
      "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ca548-140">响应</span><span class="sxs-lookup"><span data-stu-id="ca548-140">Response</span></span>
<span data-ttu-id="ca548-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca548-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




