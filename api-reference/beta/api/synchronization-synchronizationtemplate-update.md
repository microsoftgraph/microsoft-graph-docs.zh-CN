---
title: 更新 synchronizationTemplate
description: 更新 () 与给定应用程序关联的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 133f503ee6361619581cea058fbf3a47a8c7de01
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722018"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="26f73-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="26f73-103">Update synchronizationTemplate</span></span>

<span data-ttu-id="26f73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26f73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26f73-105">更新 () 与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="26f73-105">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="26f73-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="26f73-106">Permissions</span></span>
<span data-ttu-id="26f73-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f73-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26f73-109">Permission type</span></span>                        | <span data-ttu-id="26f73-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26f73-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="26f73-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26f73-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="26f73-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26f73-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="26f73-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26f73-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="26f73-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26f73-114">Not supported.</span></span>|
|<span data-ttu-id="26f73-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="26f73-115">Application</span></span>                            |<span data-ttu-id="26f73-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26f73-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="26f73-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26f73-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH applications/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="26f73-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="26f73-118">Request headers</span></span>

| <span data-ttu-id="26f73-119">名称</span><span class="sxs-lookup"><span data-stu-id="26f73-119">Name</span></span>           | <span data-ttu-id="26f73-120">类型</span><span class="sxs-lookup"><span data-stu-id="26f73-120">Type</span></span>    | <span data-ttu-id="26f73-121">说明</span><span class="sxs-lookup"><span data-stu-id="26f73-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="26f73-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26f73-122">Authorization</span></span>  | <span data-ttu-id="26f73-123">string</span><span class="sxs-lookup"><span data-stu-id="26f73-123">string</span></span>  | <span data-ttu-id="26f73-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26f73-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26f73-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26f73-126">Request body</span></span>

<span data-ttu-id="26f73-127">在请求正文中，提供 [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 对象以替换现有模板。</span><span class="sxs-lookup"><span data-stu-id="26f73-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="26f73-128">确保提供了所有属性。</span><span class="sxs-lookup"><span data-stu-id="26f73-128">Make sure all properties are provided.</span></span> <span data-ttu-id="26f73-129">将清除缺少的属性。</span><span class="sxs-lookup"><span data-stu-id="26f73-129">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="26f73-130">响应</span><span class="sxs-lookup"><span data-stu-id="26f73-130">Response</span></span>

<span data-ttu-id="26f73-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="26f73-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="26f73-133">示例</span><span class="sxs-lookup"><span data-stu-id="26f73-133">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="26f73-134">请求</span><span class="sxs-lookup"><span data-stu-id="26f73-134">Request</span></span>
<span data-ttu-id="26f73-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="26f73-135">The following is an example of a request.</span></span> 

><span data-ttu-id="26f73-136">**注意：** 为了可读性，缩短了此处所示的请求对象。</span><span class="sxs-lookup"><span data-stu-id="26f73-136">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="26f73-137">在实际调用中包括所有属性。</span><span class="sxs-lookup"><span data-stu-id="26f73-137">Include all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="26f73-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="26f73-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="26f73-139">C#</span><span class="sxs-lookup"><span data-stu-id="26f73-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26f73-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26f73-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26f73-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26f73-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26f73-142">Java</span><span class="sxs-lookup"><span data-stu-id="26f73-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26f73-143">响应</span><span class="sxs-lookup"><span data-stu-id="26f73-143">Response</span></span>
<span data-ttu-id="26f73-144">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="26f73-144">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


