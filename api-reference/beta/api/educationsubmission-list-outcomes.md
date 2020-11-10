---
title: 列表结果
description: 检索 educationoutcome 对象的列表。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5b9676e60e710ed3acd57e6719f9882f2b96d410
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965879"
---
# <a name="list-outcomes"></a><span data-ttu-id="d39eb-103">列表结果</span><span class="sxs-lookup"><span data-stu-id="d39eb-103">List outcomes</span></span>

<span data-ttu-id="d39eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d39eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d39eb-105">检索 [educationOutcome](../resources/educationoutcome.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d39eb-105">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="d39eb-106">有三种类型的结果： **educationPointsOutcome** 、 **educationFeedbackOutcome** 和 **educationRubricOutcome** 。</span><span class="sxs-lookup"><span data-stu-id="d39eb-106">There are three types of outcomes: **educationPointsOutcome** , **educationFeedbackOutcome** , and **educationRubricOutcome**.</span></span>

<span data-ttu-id="d39eb-107">对信用卡工作分配的提交 (没有磅值的人，并且没有 rubric) 将具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="d39eb-107">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="d39eb-108"> (它也可能返回 [educationPointsOutcome](../resources/educationpointsoutcome.md)，但忽略该结果。 ) </span><span class="sxs-lookup"><span data-stu-id="d39eb-108">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="d39eb-109"> () 分配了 point 值的点分配的提交将具有一个 [educationFeedbackOutcome](../resources/educationpointsoutcome.md) 和一个 [educationPointsOutcome](../resources/educationpointsoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="d39eb-109">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="d39eb-110">使用附加 rubric 的工作分配的提交。如果 rubric 是信用 rubric (没有数据点) ，将具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md) 和 [educationRubricOutcome](../resources/educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="d39eb-110">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="d39eb-111"> (它也可能返回 [educationPointsOutcome](../resources/educationpointsoutcome.md)，但忽略该结果。 ) </span><span class="sxs-lookup"><span data-stu-id="d39eb-111">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="d39eb-112">使用附加 rubric 的工作分配提交，如果 rubric 是点 rubric，则会有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)，[educationPointsOutcome] (。。/resources/educationpointsoutcome.md 和 [educationRubricOutcome](../resources/educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="d39eb-112">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="d39eb-113">所有结果类型都具有与该结果类型相对应的常规和已发布属性;例如， **点** 和 **publishedPoints** 、 **反馈** 和 **publishedFeedback** 。</span><span class="sxs-lookup"><span data-stu-id="d39eb-113">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints** , **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="d39eb-114">常规属性是教师更新的最新值;已发布的属性是返回给学生的最新值。</span><span class="sxs-lookup"><span data-stu-id="d39eb-114">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="d39eb-115">权限</span><span class="sxs-lookup"><span data-stu-id="d39eb-115">Permissions</span></span>

<span data-ttu-id="d39eb-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d39eb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d39eb-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="d39eb-118">Permission type</span></span>                        | <span data-ttu-id="d39eb-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d39eb-119">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d39eb-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d39eb-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="d39eb-121">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="d39eb-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d39eb-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d39eb-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d39eb-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="d39eb-123">Not supported.</span></span> |
| <span data-ttu-id="d39eb-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="d39eb-124">Application</span></span>                            | <span data-ttu-id="d39eb-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="d39eb-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d39eb-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d39eb-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="d39eb-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="d39eb-127">Request headers</span></span>

| <span data-ttu-id="d39eb-128">名称</span><span class="sxs-lookup"><span data-stu-id="d39eb-128">Name</span></span>      |<span data-ttu-id="d39eb-129">说明</span><span class="sxs-lookup"><span data-stu-id="d39eb-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d39eb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d39eb-130">Authorization</span></span> | <span data-ttu-id="d39eb-131">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d39eb-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d39eb-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d39eb-132">Request body</span></span>

<span data-ttu-id="d39eb-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d39eb-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d39eb-134">响应</span><span class="sxs-lookup"><span data-stu-id="d39eb-134">Response</span></span>

<span data-ttu-id="d39eb-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [educationOutcome](../resources/educationoutcome.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d39eb-135">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d39eb-136">示例</span><span class="sxs-lookup"><span data-stu-id="d39eb-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d39eb-137">请求</span><span class="sxs-lookup"><span data-stu-id="d39eb-137">Request</span></span>

<span data-ttu-id="d39eb-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d39eb-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d39eb-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d39eb-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes
```
# <a name="c"></a>[<span data-ttu-id="d39eb-140">C#</span><span class="sxs-lookup"><span data-stu-id="d39eb-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outcomes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d39eb-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d39eb-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outcomes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d39eb-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d39eb-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outcomes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d39eb-143">Java</span><span class="sxs-lookup"><span data-stu-id="d39eb-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outcomes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d39eb-144">响应</span><span class="sxs-lookup"><span data-stu-id="d39eb-144">Response</span></span>

<span data-ttu-id="d39eb-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d39eb-145">The following is an example of the response.</span></span>

> <span data-ttu-id="d39eb-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d39eb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationOutcome",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
            "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
            "feedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedFeedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationPointsOutcome",
            "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
            "points": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedPoints": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationRubricOutcome",
            "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
            "rubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "rubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ],
            "publishedRubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "publishedRubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
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
  "description": "List outcomes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


