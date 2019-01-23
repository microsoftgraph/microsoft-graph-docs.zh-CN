---
title: assign 操作
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9a9d52e62b1d4dd065c1e744593c8e63b695a526
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394360"
---
# <a name="assign-action"></a><span data-ttu-id="1e0eb-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="1e0eb-103">assign action</span></span>

> <span data-ttu-id="1e0eb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1e0eb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e0eb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e0eb-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1e0eb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e0eb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e0eb-108">Prerequisites</span></span>
<span data-ttu-id="1e0eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1e0eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e0eb-111">Permission type</span></span>|<span data-ttu-id="1e0eb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e0eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e0eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e0eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e0eb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e0eb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e0eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e0eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e0eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-116">Not supported.</span></span>|
|<span data-ttu-id="1e0eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e0eb-117">Application</span></span>|<span data-ttu-id="1e0eb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e0eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e0eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="1e0eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e0eb-120">Request headers</span></span>
|<span data-ttu-id="1e0eb-121">标头</span><span class="sxs-lookup"><span data-stu-id="1e0eb-121">Header</span></span>|<span data-ttu-id="1e0eb-122">值</span><span class="sxs-lookup"><span data-stu-id="1e0eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e0eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e0eb-123">Authorization</span></span>|<span data-ttu-id="1e0eb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e0eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e0eb-125">Accept</span></span>|<span data-ttu-id="1e0eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e0eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e0eb-127">Request body</span></span>
<span data-ttu-id="1e0eb-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1e0eb-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1e0eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="1e0eb-130">Property</span></span>|<span data-ttu-id="1e0eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="1e0eb-131">Type</span></span>|<span data-ttu-id="1e0eb-132">说明</span><span class="sxs-lookup"><span data-stu-id="1e0eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0eb-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="1e0eb-133">managedEBookAssignments</span></span>|<span data-ttu-id="1e0eb-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1e0eb-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="1e0eb-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1e0eb-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1e0eb-136">响应</span><span class="sxs-lookup"><span data-stu-id="1e0eb-136">Response</span></span>
<span data-ttu-id="1e0eb-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1e0eb-138">示例</span><span class="sxs-lookup"><span data-stu-id="1e0eb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e0eb-139">请求</span><span class="sxs-lookup"><span data-stu-id="1e0eb-139">Request</span></span>
<span data-ttu-id="1e0eb-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

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

### <a name="response"></a><span data-ttu-id="1e0eb-141">响应</span><span class="sxs-lookup"><span data-stu-id="1e0eb-141">Response</span></span>
<span data-ttu-id="1e0eb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e0eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




