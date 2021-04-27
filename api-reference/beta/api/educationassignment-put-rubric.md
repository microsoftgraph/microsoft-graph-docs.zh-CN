---
title: 将 educationRubric 附加到 educationAssignment
description: 将现有 educationRubric 对象附加到 educationAssignment。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b4ab5909a9c45947fe4f1622bb4f819fc7f3e9e5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044219"
---
# <a name="create-educationrubric"></a><span data-ttu-id="727fa-103">创建 educationRubric</span><span class="sxs-lookup"><span data-stu-id="727fa-103">Create educationRubric</span></span>

<span data-ttu-id="727fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="727fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="727fa-105">将现有的 [educationRubric](../resources/educationrubric.md) 对象附加到 [educationAssignment](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="727fa-105">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="727fa-106">权限</span><span class="sxs-lookup"><span data-stu-id="727fa-106">Permissions</span></span>

<span data-ttu-id="727fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="727fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="727fa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="727fa-109">Permission type</span></span>                        | <span data-ttu-id="727fa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="727fa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="727fa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="727fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="727fa-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="727fa-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="727fa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="727fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="727fa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="727fa-114">Not supported.</span></span> |
| <span data-ttu-id="727fa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="727fa-115">Application</span></span>                            | <span data-ttu-id="727fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="727fa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="727fa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="727fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="727fa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="727fa-118">Request headers</span></span>

| <span data-ttu-id="727fa-119">名称</span><span class="sxs-lookup"><span data-stu-id="727fa-119">Name</span></span>          | <span data-ttu-id="727fa-120">说明</span><span class="sxs-lookup"><span data-stu-id="727fa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="727fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="727fa-121">Authorization</span></span> | <span data-ttu-id="727fa-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="727fa-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="727fa-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="727fa-123">Request body</span></span>

<span data-ttu-id="727fa-124">在请求正文中，提供现有 [educationRubric](../resources/educationrubric.md) 对象的 OData ID。</span><span class="sxs-lookup"><span data-stu-id="727fa-124">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="727fa-125">响应</span><span class="sxs-lookup"><span data-stu-id="727fa-125">Response</span></span>

<span data-ttu-id="727fa-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="727fa-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="727fa-128">示例</span><span class="sxs-lookup"><span data-stu-id="727fa-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="727fa-129">请求</span><span class="sxs-lookup"><span data-stu-id="727fa-129">Request</span></span>

<span data-ttu-id="727fa-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="727fa-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="727fa-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="727fa-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="727fa-132">C#</span><span class="sxs-lookup"><span data-stu-id="727fa-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="727fa-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="727fa-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="727fa-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="727fa-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="727fa-135">Java</span><span class="sxs-lookup"><span data-stu-id="727fa-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="727fa-136">响应</span><span class="sxs-lookup"><span data-stu-id="727fa-136">Response</span></span>

<span data-ttu-id="727fa-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="727fa-137">The following is an example of the response.</span></span>

> <span data-ttu-id="727fa-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="727fa-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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


