---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 967336fc159e7e6620ec760f4f37b29c6f4574ae
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538019"
---
# <a name="assign-action"></a><span data-ttu-id="d42f9-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="d42f9-103">assign action</span></span>

> <span data-ttu-id="d42f9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d42f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d42f9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d42f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d42f9-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d42f9-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d42f9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d42f9-107">Prerequisites</span></span>
<span data-ttu-id="d42f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d42f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d42f9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d42f9-110">Permission type</span></span>|<span data-ttu-id="d42f9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d42f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d42f9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d42f9-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d42f9-113">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="d42f9-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d42f9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d42f9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d42f9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d42f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d42f9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d42f9-116">Not supported.</span></span>|
|<span data-ttu-id="d42f9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d42f9-117">Application</span></span>||
| <span data-ttu-id="d42f9-118">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="d42f9-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d42f9-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d42f9-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d42f9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d42f9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="d42f9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d42f9-121">Request headers</span></span>
|<span data-ttu-id="d42f9-122">标头</span><span class="sxs-lookup"><span data-stu-id="d42f9-122">Header</span></span>|<span data-ttu-id="d42f9-123">值</span><span class="sxs-lookup"><span data-stu-id="d42f9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d42f9-124">授权</span><span class="sxs-lookup"><span data-stu-id="d42f9-124">Authorization</span></span>|<span data-ttu-id="d42f9-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d42f9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d42f9-126">接受</span><span class="sxs-lookup"><span data-stu-id="d42f9-126">Accept</span></span>|<span data-ttu-id="d42f9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d42f9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d42f9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d42f9-128">Request body</span></span>
<span data-ttu-id="d42f9-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d42f9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d42f9-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d42f9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d42f9-131">属性</span><span class="sxs-lookup"><span data-stu-id="d42f9-131">Property</span></span>|<span data-ttu-id="d42f9-132">类型</span><span class="sxs-lookup"><span data-stu-id="d42f9-132">Type</span></span>|<span data-ttu-id="d42f9-133">说明</span><span class="sxs-lookup"><span data-stu-id="d42f9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d42f9-134">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="d42f9-134">mobileAppAssignments</span></span>|<span data-ttu-id="d42f9-135">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d42f9-135">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="d42f9-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d42f9-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d42f9-137">响应</span><span class="sxs-lookup"><span data-stu-id="d42f9-137">Response</span></span>
<span data-ttu-id="d42f9-138">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d42f9-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d42f9-139">示例</span><span class="sxs-lookup"><span data-stu-id="d42f9-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d42f9-140">请求</span><span class="sxs-lookup"><span data-stu-id="d42f9-140">Request</span></span>
<span data-ttu-id="d42f9-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d42f9-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d42f9-142">响应</span><span class="sxs-lookup"><span data-stu-id="d42f9-142">Response</span></span>
<span data-ttu-id="d42f9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d42f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






