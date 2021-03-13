---
title: 创建 synchronizationTemplate
description: 为给定应用程序创建新的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b2c501d0c07e91aa3b0dbb707320f4909db299de
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50775428"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="4be77-103">创建 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="4be77-103">Create synchronizationTemplate</span></span>

<span data-ttu-id="4be77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4be77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be77-105">为给定应用程序创建新的同步模板。</span><span class="sxs-lookup"><span data-stu-id="4be77-105">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="4be77-106">权限</span><span class="sxs-lookup"><span data-stu-id="4be77-106">Permissions</span></span>
<span data-ttu-id="4be77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4be77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be77-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4be77-109">Permission type</span></span>                        | <span data-ttu-id="4be77-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4be77-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be77-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4be77-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="4be77-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be77-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4be77-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4be77-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4be77-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4be77-114">Not supported.</span></span>|
|<span data-ttu-id="4be77-115">Application</span><span class="sxs-lookup"><span data-stu-id="4be77-115">Application</span></span>                            |<span data-ttu-id="4be77-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be77-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="4be77-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4be77-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="4be77-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4be77-118">Request headers</span></span>

| <span data-ttu-id="4be77-119">名称</span><span class="sxs-lookup"><span data-stu-id="4be77-119">Name</span></span>           | <span data-ttu-id="4be77-120">类型</span><span class="sxs-lookup"><span data-stu-id="4be77-120">Type</span></span>    | <span data-ttu-id="4be77-121">说明</span><span class="sxs-lookup"><span data-stu-id="4be77-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4be77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4be77-122">Authorization</span></span>  | <span data-ttu-id="4be77-123">string</span><span class="sxs-lookup"><span data-stu-id="4be77-123">string</span></span>  | <span data-ttu-id="4be77-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4be77-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4be77-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4be77-126">Request body</span></span>

<span data-ttu-id="4be77-127">在请求正文中，提供 [要创建的 synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4be77-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="4be77-128">`id`和 `applicationId` `factoryTag` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="4be77-128">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="4be77-129">如果 `schema` 模板未提供，则使用与 属性关联的 `factoryTag` 默认架构。</span><span class="sxs-lookup"><span data-stu-id="4be77-129">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="4be77-130">响应</span><span class="sxs-lookup"><span data-stu-id="4be77-130">Response</span></span>

<span data-ttu-id="4be77-131">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4be77-131">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="4be77-132">示例</span><span class="sxs-lookup"><span data-stu-id="4be77-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4be77-133">请求</span><span class="sxs-lookup"><span data-stu-id="4be77-133">Request</span></span>
<span data-ttu-id="4be77-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="4be77-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4be77-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4be77-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="c"></a>[<span data-ttu-id="4be77-136">C#</span><span class="sxs-lookup"><span data-stu-id="4be77-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4be77-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4be77-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4be77-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4be77-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4be77-139">Java</span><span class="sxs-lookup"><span data-stu-id="4be77-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationtemplate-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4be77-140">响应</span><span class="sxs-lookup"><span data-stu-id="4be77-140">Response</span></span>
<span data-ttu-id="4be77-141">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="4be77-141">The following is an example of a response.</span></span>
><span data-ttu-id="4be77-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4be77-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4be77-143">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4be77-143">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


