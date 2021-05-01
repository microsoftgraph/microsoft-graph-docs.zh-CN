---
title: 更新 educationRubric
description: 更新 educationRubric 对象的属性。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 50e3d9a675a6052f6eb2f26b5ed28a3395b77063
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118988"
---
# <a name="update-educationrubric"></a><span data-ttu-id="bcd53-103">更新 educationRubric</span><span class="sxs-lookup"><span data-stu-id="bcd53-103">Update educationRubric</span></span>

<span data-ttu-id="bcd53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcd53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcd53-105">更新 [educationRubric 对象](../resources/educationrubric.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="bcd53-105">Update the properties of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="bcd53-106">只有在发布工作分配 () 工作分配附加的一个分值才能更新，而更新的实际上是 下 `PATCH /education/classes/{id}/assignments/{id}/rubric` 的原始工作分配 `/education/users/{id}/rubrics` 。</span><span class="sxs-lookup"><span data-stu-id="bcd53-106">Updating a rubric attached to an assignment (`PATCH /education/classes/{id}/assignments/{id}/rubric`) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="bcd53-107">工作分配发布后，将创建附加到该特定工作分配的不可变重复副本。</span><span class="sxs-lookup"><span data-stu-id="bcd53-107">After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment.</span></span> <span data-ttu-id="bcd53-108">可以使用 [GET /education/classes/{id}/assignments/{id}/rubric](educationrubric-get.md)检索该标准，但无法更新。</span><span class="sxs-lookup"><span data-stu-id="bcd53-108">That rubric can be retrieved using [GET /education/classes/{id}/assignments/{id}/rubric](educationrubric-get.md), but it cannot be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcd53-109">权限</span><span class="sxs-lookup"><span data-stu-id="bcd53-109">Permissions</span></span>

<span data-ttu-id="bcd53-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcd53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bcd53-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcd53-112">Permission type</span></span>                        | <span data-ttu-id="bcd53-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcd53-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bcd53-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcd53-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="bcd53-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcd53-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="bcd53-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcd53-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcd53-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcd53-117">Not supported.</span></span> |
| <span data-ttu-id="bcd53-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcd53-118">Application</span></span>                            | <span data-ttu-id="bcd53-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcd53-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcd53-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcd53-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me/rubrics/{id}
PATCH /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="bcd53-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcd53-121">Request headers</span></span>

| <span data-ttu-id="bcd53-122">名称</span><span class="sxs-lookup"><span data-stu-id="bcd53-122">Name</span></span>       | <span data-ttu-id="bcd53-123">说明</span><span class="sxs-lookup"><span data-stu-id="bcd53-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bcd53-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcd53-124">Authorization</span></span> | <span data-ttu-id="bcd53-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="bcd53-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcd53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcd53-126">Request body</span></span>

<span data-ttu-id="bcd53-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bcd53-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bcd53-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bcd53-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bcd53-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bcd53-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bcd53-130">属性</span><span class="sxs-lookup"><span data-stu-id="bcd53-130">Property</span></span>     | <span data-ttu-id="bcd53-131">类型</span><span class="sxs-lookup"><span data-stu-id="bcd53-131">Type</span></span>        | <span data-ttu-id="bcd53-132">说明</span><span class="sxs-lookup"><span data-stu-id="bcd53-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bcd53-133">说明</span><span class="sxs-lookup"><span data-stu-id="bcd53-133">description</span></span>|<span data-ttu-id="bcd53-134">itemBody</span><span class="sxs-lookup"><span data-stu-id="bcd53-134">itemBody</span></span>|<span data-ttu-id="bcd53-135">此分卡的说明。</span><span class="sxs-lookup"><span data-stu-id="bcd53-135">The description of this rubric.</span></span>|
|<span data-ttu-id="bcd53-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bcd53-136">displayName</span></span>|<span data-ttu-id="bcd53-137">字符串</span><span class="sxs-lookup"><span data-stu-id="bcd53-137">String</span></span>|<span data-ttu-id="bcd53-138">此分号的名称。</span><span class="sxs-lookup"><span data-stu-id="bcd53-138">The name of this rubric.</span></span>|
|<span data-ttu-id="bcd53-139">一个</span><span class="sxs-lookup"><span data-stu-id="bcd53-139">grading</span></span>|<span data-ttu-id="bcd53-140">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="bcd53-140">educationAssignmentGradeType</span></span>|<span data-ttu-id="bcd53-141">此分值是否具有点。</span><span class="sxs-lookup"><span data-stu-id="bcd53-141">Whether this rubric has points or not.</span></span>|
|<span data-ttu-id="bcd53-142">levels</span><span class="sxs-lookup"><span data-stu-id="bcd53-142">levels</span></span>|<span data-ttu-id="bcd53-143">rubricLevel 集合</span><span class="sxs-lookup"><span data-stu-id="bcd53-143">rubricLevel collection</span></span>|<span data-ttu-id="bcd53-144">此标准中的级别集合。</span><span class="sxs-lookup"><span data-stu-id="bcd53-144">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="bcd53-145">一些</span><span class="sxs-lookup"><span data-stu-id="bcd53-145">qualities</span></span>|<span data-ttu-id="bcd53-146">rubricQuality 集合</span><span class="sxs-lookup"><span data-stu-id="bcd53-146">rubricQuality collection</span></span>|<span data-ttu-id="bcd53-147">此分项由质量集合决定。</span><span class="sxs-lookup"><span data-stu-id="bcd53-147">The collection of qualities making up this rubric.</span></span>|

## <a name="response"></a><span data-ttu-id="bcd53-148">响应</span><span class="sxs-lookup"><span data-stu-id="bcd53-148">Response</span></span>

<span data-ttu-id="bcd53-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationRubric](../resources/educationrubric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bcd53-149">If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bcd53-150">示例</span><span class="sxs-lookup"><span data-stu-id="bcd53-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bcd53-151">请求</span><span class="sxs-lookup"><span data-stu-id="bcd53-151">Request</span></span>

<span data-ttu-id="bcd53-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bcd53-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcd53-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcd53-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/rubrics/{id}
Content-type: application/json

{
  "displayName": "Example Credit Rubric after display name patch"
}
```
# <a name="c"></a>[<span data-ttu-id="bcd53-154">C#</span><span class="sxs-lookup"><span data-stu-id="bcd53-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcd53-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcd53-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcd53-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcd53-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcd53-157">Java</span><span class="sxs-lookup"><span data-stu-id="bcd53-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationrubric-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bcd53-158">响应</span><span class="sxs-lookup"><span data-stu-id="bcd53-158">Response</span></span>

<span data-ttu-id="bcd53-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bcd53-159">The following is an example of the response.</span></span>

> <span data-ttu-id="bcd53-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bcd53-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "displayName": "Example Credit Rubric after display name patch",
    "id": "c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f2e4b0f-508e-4005-984b-17e061bc5377",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "dc79dcbf-b536-4797-9c5b-902f28129fd0",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "7e087062-ac25-4629-8386-a946350936db",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "12276eb2-122c-4ad2-ba92-335ea798c88e",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationrubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


