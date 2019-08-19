---
title: 将 educationRubric 附加到 educationAssignment
description: 将现有的 educationRubric 对象附加到 educationAssignment。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 84a0f60edfa292776291e823538c45ae7e7d5898
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461141"
---
# <a name="create-educationrubric"></a><span data-ttu-id="4fd0d-103">创建 educationRubric</span><span class="sxs-lookup"><span data-stu-id="4fd0d-103">Create educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fd0d-104">将现有的[educationRubric](../resources/educationrubric.md)对象附加到[educationAssignment](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-104">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4fd0d-105">权限</span><span class="sxs-lookup"><span data-stu-id="4fd0d-105">Permissions</span></span>

<span data-ttu-id="4fd0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fd0d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fd0d-108">Permission type</span></span>                        | <span data-ttu-id="4fd0d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fd0d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4fd0d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fd0d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fd0d-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="4fd0d-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="4fd0d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fd0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fd0d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-113">Not supported.</span></span> |
| <span data-ttu-id="4fd0d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fd0d-114">Application</span></span>                            | <span data-ttu-id="4fd0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fd0d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fd0d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4fd0d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fd0d-117">Request headers</span></span>

| <span data-ttu-id="4fd0d-118">名称</span><span class="sxs-lookup"><span data-stu-id="4fd0d-118">Name</span></span>          | <span data-ttu-id="4fd0d-119">说明</span><span class="sxs-lookup"><span data-stu-id="4fd0d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4fd0d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fd0d-120">Authorization</span></span> | <span data-ttu-id="4fd0d-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4fd0d-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fd0d-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fd0d-122">Request body</span></span>

<span data-ttu-id="4fd0d-123">在请求正文中, 提供现有[educationRubric](../resources/educationrubric.md)对象的 OData ID。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-123">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4fd0d-124">响应</span><span class="sxs-lookup"><span data-stu-id="4fd0d-124">Response</span></span>

<span data-ttu-id="4fd0d-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fd0d-127">示例</span><span class="sxs-lookup"><span data-stu-id="4fd0d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fd0d-128">请求</span><span class="sxs-lookup"><span data-stu-id="4fd0d-128">Request</span></span>

<span data-ttu-id="4fd0d-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4fd0d-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4fd0d-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4fd0d-131">C#</span><span class="sxs-lookup"><span data-stu-id="4fd0d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fd0d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fd0d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4fd0d-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="4fd0d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4fd0d-134">响应</span><span class="sxs-lookup"><span data-stu-id="4fd0d-134">Response</span></span>

<span data-ttu-id="4fd0d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-135">The following is an example of the response.</span></span>

> <span data-ttu-id="4fd0d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4fd0d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
