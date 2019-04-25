---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94c50cf4e3f880f61f1e392d9166c6dfe7a6f5ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524905"
---
# <a name="assign-action"></a><span data-ttu-id="a8df8-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="a8df8-103">assign action</span></span>

> <span data-ttu-id="a8df8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8df8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8df8-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a8df8-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8df8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8df8-106">Prerequisites</span></span>
<span data-ttu-id="a8df8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8df8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8df8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8df8-109">Permission type</span></span>|<span data-ttu-id="a8df8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8df8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8df8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8df8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8df8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8df8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8df8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8df8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8df8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8df8-114">Not supported.</span></span>|
|<span data-ttu-id="a8df8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8df8-115">Application</span></span>|<span data-ttu-id="a8df8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8df8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8df8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8df8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a8df8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8df8-118">Request headers</span></span>
|<span data-ttu-id="a8df8-119">标头</span><span class="sxs-lookup"><span data-stu-id="a8df8-119">Header</span></span>|<span data-ttu-id="a8df8-120">值</span><span class="sxs-lookup"><span data-stu-id="a8df8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8df8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8df8-121">Authorization</span></span>|<span data-ttu-id="a8df8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8df8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8df8-123">接受</span><span class="sxs-lookup"><span data-stu-id="a8df8-123">Accept</span></span>|<span data-ttu-id="a8df8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a8df8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8df8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8df8-125">Request body</span></span>
<span data-ttu-id="a8df8-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8df8-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a8df8-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a8df8-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a8df8-128">属性</span><span class="sxs-lookup"><span data-stu-id="a8df8-128">Property</span></span>|<span data-ttu-id="a8df8-129">类型</span><span class="sxs-lookup"><span data-stu-id="a8df8-129">Type</span></span>|<span data-ttu-id="a8df8-130">说明</span><span class="sxs-lookup"><span data-stu-id="a8df8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8df8-131">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="a8df8-131">managedEBookAssignments</span></span>|<span data-ttu-id="a8df8-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8df8-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="a8df8-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a8df8-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a8df8-134">响应</span><span class="sxs-lookup"><span data-stu-id="a8df8-134">Response</span></span>
<span data-ttu-id="a8df8-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a8df8-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8df8-136">示例</span><span class="sxs-lookup"><span data-stu-id="a8df8-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8df8-137">请求</span><span class="sxs-lookup"><span data-stu-id="a8df8-137">Request</span></span>
<span data-ttu-id="a8df8-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8df8-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8df8-139">响应</span><span class="sxs-lookup"><span data-stu-id="a8df8-139">Response</span></span>
<span data-ttu-id="a8df8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8df8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



