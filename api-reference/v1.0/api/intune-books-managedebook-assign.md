---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71c6237392e96347f3ee207311afe91b362c4c29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018482"
---
# <a name="assign-action"></a><span data-ttu-id="c7ad7-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="c7ad7-103">assign action</span></span>

> <span data-ttu-id="c7ad7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7ad7-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7ad7-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7ad7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7ad7-106">Prerequisites</span></span>
<span data-ttu-id="c7ad7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ad7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7ad7-109">Permission type</span></span>|<span data-ttu-id="c7ad7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7ad7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7ad7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7ad7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7ad7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ad7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7ad7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7ad7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7ad7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-114">Not supported.</span></span>|
|<span data-ttu-id="c7ad7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7ad7-115">Application</span></span>|<span data-ttu-id="c7ad7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7ad7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7ad7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c7ad7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7ad7-118">Request headers</span></span>
|<span data-ttu-id="c7ad7-119">标头</span><span class="sxs-lookup"><span data-stu-id="c7ad7-119">Header</span></span>|<span data-ttu-id="c7ad7-120">值</span><span class="sxs-lookup"><span data-stu-id="c7ad7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7ad7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7ad7-121">Authorization</span></span>|<span data-ttu-id="c7ad7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7ad7-123">接受</span><span class="sxs-lookup"><span data-stu-id="c7ad7-123">Accept</span></span>|<span data-ttu-id="c7ad7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c7ad7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7ad7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7ad7-125">Request body</span></span>
<span data-ttu-id="c7ad7-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c7ad7-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c7ad7-128">属性</span><span class="sxs-lookup"><span data-stu-id="c7ad7-128">Property</span></span>|<span data-ttu-id="c7ad7-129">类型</span><span class="sxs-lookup"><span data-stu-id="c7ad7-129">Type</span></span>|<span data-ttu-id="c7ad7-130">说明</span><span class="sxs-lookup"><span data-stu-id="c7ad7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ad7-131">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="c7ad7-131">managedEBookAssignments</span></span>|<span data-ttu-id="c7ad7-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7ad7-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="c7ad7-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7ad7-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c7ad7-134">响应</span><span class="sxs-lookup"><span data-stu-id="c7ad7-134">Response</span></span>
<span data-ttu-id="c7ad7-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c7ad7-136">示例</span><span class="sxs-lookup"><span data-stu-id="c7ad7-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7ad7-137">请求</span><span class="sxs-lookup"><span data-stu-id="c7ad7-137">Request</span></span>
<span data-ttu-id="c7ad7-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 318

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c7ad7-139">响应</span><span class="sxs-lookup"><span data-stu-id="c7ad7-139">Response</span></span>
<span data-ttu-id="c7ad7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7ad7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



