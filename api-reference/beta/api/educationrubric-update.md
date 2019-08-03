---
title: 更新 educationRubric
description: 更新 educationRubric 对象的属性。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c1c900084c0410f583621b43b145ccd9934c820b
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173137"
---
# <a name="update-educationrubric"></a><span data-ttu-id="0d696-103">更新 educationRubric</span><span class="sxs-lookup"><span data-stu-id="0d696-103">Update educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d696-104">更新[educationRubric](../resources/educationrubric.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0d696-104">Update the properties of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="0d696-105">仅在发布工作分配之前可以更新`PATCH /education/me/assignments/{id}/rubric`附加到工作分配的 rubric (), 而更新的内容实际上是`/education/users/{id}/rubrics`中存在的原始 rubric。</span><span class="sxs-lookup"><span data-stu-id="0d696-105">Updating a rubric attached to an assignment (`PATCH /education/me/assignments/{id}/rubric`) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="0d696-106">发布工作分配后, 将创建一个 rubric 的不可变副本, 该副本将附加到该特定工作分配。</span><span class="sxs-lookup"><span data-stu-id="0d696-106">After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment.</span></span> <span data-ttu-id="0d696-107">可以使用[GET/education/me/assignments/{id}/rubric](educationrubric-get.md)检索 rubric, 但不能对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="0d696-107">That rubric can be retrieved using [GET /education/me/assignments/{id}/rubric](educationrubric-get.md), but it cannot be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d696-108">权限</span><span class="sxs-lookup"><span data-stu-id="0d696-108">Permissions</span></span>

<span data-ttu-id="0d696-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d696-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d696-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d696-111">Permission type</span></span>                        | <span data-ttu-id="0d696-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d696-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d696-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d696-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d696-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0d696-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="0d696-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d696-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d696-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d696-116">Not supported.</span></span> |
| <span data-ttu-id="0d696-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d696-117">Application</span></span>                            | <span data-ttu-id="0d696-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d696-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d696-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d696-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me/rubrics/{id}
PATCH /education/me/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="0d696-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d696-120">Request headers</span></span>

| <span data-ttu-id="0d696-121">名称</span><span class="sxs-lookup"><span data-stu-id="0d696-121">Name</span></span>       | <span data-ttu-id="0d696-122">说明</span><span class="sxs-lookup"><span data-stu-id="0d696-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0d696-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d696-123">Authorization</span></span> | <span data-ttu-id="0d696-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0d696-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d696-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d696-125">Request body</span></span>

<span data-ttu-id="0d696-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0d696-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0d696-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0d696-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0d696-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0d696-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d696-129">属性</span><span class="sxs-lookup"><span data-stu-id="0d696-129">Property</span></span>     | <span data-ttu-id="0d696-130">类型</span><span class="sxs-lookup"><span data-stu-id="0d696-130">Type</span></span>        | <span data-ttu-id="0d696-131">说明</span><span class="sxs-lookup"><span data-stu-id="0d696-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d696-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d696-132">description</span></span>|<span data-ttu-id="0d696-133">itemBody</span><span class="sxs-lookup"><span data-stu-id="0d696-133">itemBody</span></span>|<span data-ttu-id="0d696-134">此 rubric 的说明。</span><span class="sxs-lookup"><span data-stu-id="0d696-134">The description of this rubric.</span></span>|
|<span data-ttu-id="0d696-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0d696-135">displayName</span></span>|<span data-ttu-id="0d696-136">String</span><span class="sxs-lookup"><span data-stu-id="0d696-136">String</span></span>|<span data-ttu-id="0d696-137">此 rubric 的名称。</span><span class="sxs-lookup"><span data-stu-id="0d696-137">The name of this rubric.</span></span>|
|<span data-ttu-id="0d696-138">评分</span><span class="sxs-lookup"><span data-stu-id="0d696-138">grading</span></span>|<span data-ttu-id="0d696-139">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="0d696-139">educationAssignmentGradeType</span></span>|<span data-ttu-id="0d696-140">此 rubric 是否有积分。</span><span class="sxs-lookup"><span data-stu-id="0d696-140">Whether this rubric has points or not.</span></span>|
|<span data-ttu-id="0d696-141">等级</span><span class="sxs-lookup"><span data-stu-id="0d696-141">levels</span></span>|<span data-ttu-id="0d696-142">rubricLevel 集合</span><span class="sxs-lookup"><span data-stu-id="0d696-142">rubricLevel collection</span></span>|<span data-ttu-id="0d696-143">构成此 rubric 的级别的集合。</span><span class="sxs-lookup"><span data-stu-id="0d696-143">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="0d696-144">特质</span><span class="sxs-lookup"><span data-stu-id="0d696-144">qualities</span></span>|<span data-ttu-id="0d696-145">rubricQuality 集合</span><span class="sxs-lookup"><span data-stu-id="0d696-145">rubricQuality collection</span></span>|<span data-ttu-id="0d696-146">构成此 rubric 的质量的集合。</span><span class="sxs-lookup"><span data-stu-id="0d696-146">The collection of qualities making up this rubric.</span></span>|

## <a name="response"></a><span data-ttu-id="0d696-147">响应</span><span class="sxs-lookup"><span data-stu-id="0d696-147">Response</span></span>

<span data-ttu-id="0d696-148">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0d696-148">If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d696-149">示例</span><span class="sxs-lookup"><span data-stu-id="0d696-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d696-150">请求</span><span class="sxs-lookup"><span data-stu-id="0d696-150">Request</span></span>

<span data-ttu-id="0d696-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d696-151">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d696-152">响应</span><span class="sxs-lookup"><span data-stu-id="0d696-152">Response</span></span>

<span data-ttu-id="0d696-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d696-153">The following is an example of the response.</span></span>

> <span data-ttu-id="0d696-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d696-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
