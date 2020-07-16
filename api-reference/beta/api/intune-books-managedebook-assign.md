---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbe825eae1ac6fe8d5af5cef347a30fe3340956b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793211"
---
# <a name="assign-action"></a><span data-ttu-id="53f93-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="53f93-103">assign action</span></span>

<span data-ttu-id="53f93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53f93-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53f93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53f93-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53f93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53f93-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="53f93-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53f93-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="53f93-108">Prerequisites</span></span>
<span data-ttu-id="53f93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53f93-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53f93-111">Permission type</span></span>|<span data-ttu-id="53f93-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53f93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53f93-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53f93-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f93-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53f93-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53f93-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53f93-116">Not supported.</span></span>|
|<span data-ttu-id="53f93-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53f93-117">Application</span></span>|<span data-ttu-id="53f93-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f93-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53f93-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="53f93-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53f93-120">Request headers</span></span>
|<span data-ttu-id="53f93-121">标头</span><span class="sxs-lookup"><span data-stu-id="53f93-121">Header</span></span>|<span data-ttu-id="53f93-122">值</span><span class="sxs-lookup"><span data-stu-id="53f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53f93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53f93-123">Authorization</span></span>|<span data-ttu-id="53f93-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53f93-125">接受</span><span class="sxs-lookup"><span data-stu-id="53f93-125">Accept</span></span>|<span data-ttu-id="53f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53f93-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53f93-127">Request body</span></span>
<span data-ttu-id="53f93-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53f93-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="53f93-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="53f93-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="53f93-130">属性</span><span class="sxs-lookup"><span data-stu-id="53f93-130">Property</span></span>|<span data-ttu-id="53f93-131">类型</span><span class="sxs-lookup"><span data-stu-id="53f93-131">Type</span></span>|<span data-ttu-id="53f93-132">说明</span><span class="sxs-lookup"><span data-stu-id="53f93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53f93-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="53f93-133">managedEBookAssignments</span></span>|<span data-ttu-id="53f93-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53f93-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="53f93-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="53f93-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="53f93-136">响应</span><span class="sxs-lookup"><span data-stu-id="53f93-136">Response</span></span>
<span data-ttu-id="53f93-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="53f93-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="53f93-138">示例</span><span class="sxs-lookup"><span data-stu-id="53f93-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="53f93-139">请求</span><span class="sxs-lookup"><span data-stu-id="53f93-139">Request</span></span>
<span data-ttu-id="53f93-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53f93-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 487

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="53f93-141">响应</span><span class="sxs-lookup"><span data-stu-id="53f93-141">Response</span></span>
<span data-ttu-id="53f93-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53f93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



