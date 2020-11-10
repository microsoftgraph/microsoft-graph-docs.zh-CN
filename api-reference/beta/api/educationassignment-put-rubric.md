---
title: 将 educationRubric 附加到 educationAssignment
description: 将现有的 educationRubric 对象附加到 educationAssignment。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3d96ca954dbfb40c5c3db1f8404144337bcc0f34
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966499"
---
# <a name="create-educationrubric"></a><span data-ttu-id="05b0f-103">创建 educationRubric</span><span class="sxs-lookup"><span data-stu-id="05b0f-103">Create educationRubric</span></span>

<span data-ttu-id="05b0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05b0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05b0f-105">将现有的 [educationRubric](../resources/educationrubric.md) 对象附加到 [educationAssignment](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="05b0f-105">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05b0f-106">权限</span><span class="sxs-lookup"><span data-stu-id="05b0f-106">Permissions</span></span>

<span data-ttu-id="05b0f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05b0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05b0f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05b0f-109">Permission type</span></span>                        | <span data-ttu-id="05b0f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05b0f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05b0f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05b0f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05b0f-112">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="05b0f-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="05b0f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05b0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05b0f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05b0f-114">Not supported.</span></span> |
| <span data-ttu-id="05b0f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05b0f-115">Application</span></span>                            | <span data-ttu-id="05b0f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05b0f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05b0f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05b0f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="05b0f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="05b0f-118">Request headers</span></span>

| <span data-ttu-id="05b0f-119">名称</span><span class="sxs-lookup"><span data-stu-id="05b0f-119">Name</span></span>          | <span data-ttu-id="05b0f-120">说明</span><span class="sxs-lookup"><span data-stu-id="05b0f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="05b0f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05b0f-121">Authorization</span></span> | <span data-ttu-id="05b0f-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="05b0f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="05b0f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="05b0f-123">Request body</span></span>

<span data-ttu-id="05b0f-124">在请求正文中，提供现有 [educationRubric](../resources/educationrubric.md) 对象的 OData ID。</span><span class="sxs-lookup"><span data-stu-id="05b0f-124">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="05b0f-125">响应</span><span class="sxs-lookup"><span data-stu-id="05b0f-125">Response</span></span>

<span data-ttu-id="05b0f-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="05b0f-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05b0f-128">示例</span><span class="sxs-lookup"><span data-stu-id="05b0f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05b0f-129">请求</span><span class="sxs-lookup"><span data-stu-id="05b0f-129">Request</span></span>

<span data-ttu-id="05b0f-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05b0f-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05b0f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="05b0f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationassignment"
}-->

```http
PUT https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="05b0f-132">C#</span><span class="sxs-lookup"><span data-stu-id="05b0f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05b0f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05b0f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05b0f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05b0f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05b0f-135">Java</span><span class="sxs-lookup"><span data-stu-id="05b0f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05b0f-136">响应</span><span class="sxs-lookup"><span data-stu-id="05b0f-136">Response</span></span>

<span data-ttu-id="05b0f-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="05b0f-137">The following is an example of the response.</span></span>

> <span data-ttu-id="05b0f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="05b0f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


