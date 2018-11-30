---
title: 更新 synchronizationTemplate
description: 更新 （覆盖） 与给定应用程序关联的同步模板。
ms.openlocfilehash: 9862b0a31294448e1b43e8438b76a16d471cb2d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048590"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="dafb4-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="dafb4-103">Update synchronizationTemplate</span></span>

> <span data-ttu-id="dafb4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dafb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dafb4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dafb4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dafb4-106">更新 （覆盖） 与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="dafb4-106">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="dafb4-107">权限</span><span class="sxs-lookup"><span data-stu-id="dafb4-107">Permissions</span></span>
<span data-ttu-id="dafb4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dafb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dafb4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dafb4-110">Permission type</span></span>                        | <span data-ttu-id="dafb4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dafb4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dafb4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dafb4-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="dafb4-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dafb4-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="dafb4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dafb4-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="dafb4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dafb4-115">Not supported.</span></span>|
|<span data-ttu-id="dafb4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dafb4-116">Application</span></span>                            |<span data-ttu-id="dafb4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dafb4-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="dafb4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dafb4-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="dafb4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dafb4-119">Request headers</span></span>

| <span data-ttu-id="dafb4-120">名称</span><span class="sxs-lookup"><span data-stu-id="dafb4-120">Name</span></span>           | <span data-ttu-id="dafb4-121">类型</span><span class="sxs-lookup"><span data-stu-id="dafb4-121">Type</span></span>    | <span data-ttu-id="dafb4-122">说明</span><span class="sxs-lookup"><span data-stu-id="dafb4-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="dafb4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dafb4-123">Authorization</span></span>  | <span data-ttu-id="dafb4-124">string</span><span class="sxs-lookup"><span data-stu-id="dafb4-124">string</span></span>  | <span data-ttu-id="dafb4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dafb4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dafb4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dafb4-127">Request body</span></span>

<span data-ttu-id="dafb4-128">在请求正文中，提供要替换现有模板的[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dafb4-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="dafb4-129">确保提供了所有属性。</span><span class="sxs-lookup"><span data-stu-id="dafb4-129">Make sure all properties are provided.</span></span> <span data-ttu-id="dafb4-130">缺少的属性将被清除。</span><span class="sxs-lookup"><span data-stu-id="dafb4-130">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="dafb4-131">响应</span><span class="sxs-lookup"><span data-stu-id="dafb4-131">Response</span></span>

<span data-ttu-id="dafb4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dafb4-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="dafb4-134">示例</span><span class="sxs-lookup"><span data-stu-id="dafb4-134">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="dafb4-135">请求</span><span class="sxs-lookup"><span data-stu-id="dafb4-135">Request</span></span>
<span data-ttu-id="dafb4-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dafb4-136">The following is an example of a request.</span></span> 

><span data-ttu-id="dafb4-137">**注意：** 为便于阅读将被截如下所示的请求对象。</span><span class="sxs-lookup"><span data-stu-id="dafb4-137">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="dafb4-138">在实际呼叫中包含的所有属性。</span><span class="sxs-lookup"><span data-stu-id="dafb4-138">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="dafb4-139">响应</span><span class="sxs-lookup"><span data-stu-id="dafb4-139">Response</span></span>
<span data-ttu-id="dafb4-140">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="dafb4-140">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->