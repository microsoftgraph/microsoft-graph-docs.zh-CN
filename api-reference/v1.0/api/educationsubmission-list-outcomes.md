---
title: 列出结果
description: 检索 educationoutcome 对象的列表。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5813e5628e1ff9819cd2d10dd502d8a717088611
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992610"
---
# <a name="list-outcomes"></a><span data-ttu-id="e5be0-103">列出结果</span><span class="sxs-lookup"><span data-stu-id="e5be0-103">List outcomes</span></span>

<span data-ttu-id="e5be0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5be0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5be0-105">检索 [educationOutcome 对象](../resources/educationoutcome.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="e5be0-105">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="e5be0-106">有三种类型的结果 **：educationPointsOutcome、educationFeedbackOutcome** 和 **educationRubricOutcome**。 </span><span class="sxs-lookup"><span data-stu-id="e5be0-106">There are three types of outcomes: **educationPointsOutcome**, **educationFeedbackOutcome**, and **educationRubricOutcome**.</span></span>

<span data-ttu-id="e5be0-107">对于没有点值和 (信用额度的信用分配提交) 将具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="e5be0-107">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="e5be0-108"> (它也可能返回 [educationPointsOutcome](../resources/educationpointsoutcome.md)，但会忽略该结果。) </span><span class="sxs-lookup"><span data-stu-id="e5be0-108">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="e5be0-109">分数分配提交 (分配了分数值的) 将同时具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md) 和 [educationPointsOutcome](../resources/educationpointsoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="e5be0-109">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="e5be0-110">具有附加的分数的作业提交（如果分数为信用额度 (无分数) ，则具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md) 和 [educationRubricOutcome](../resources/educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="e5be0-110">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="e5be0-111"> (它也可能返回 [educationPointsOutcome](../resources/educationpointsoutcome.md)，但会忽略该结果。) </span><span class="sxs-lookup"><span data-stu-id="e5be0-111">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="e5be0-112">对于附加了标点的工作分配，如果分数为分值，则提交内容将具有 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)，即 [educationPointsOutcome] (。/resources/educationpointsoutcome.md 和 [educationRubricOutcome](../resources/educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="e5be0-112">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="e5be0-113">所有结果类型都有一个适合该结果类型的常规和已发布属性;例如 **，points** 和 **publishedPoints** **、feedback** 和 **publishedFeedback**。</span><span class="sxs-lookup"><span data-stu-id="e5be0-113">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="e5be0-114">常规属性是由教师更新的最新值;已发布属性是返回到学生的最新值。</span><span class="sxs-lookup"><span data-stu-id="e5be0-114">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5be0-115">权限</span><span class="sxs-lookup"><span data-stu-id="e5be0-115">Permissions</span></span>

<span data-ttu-id="e5be0-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5be0-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5be0-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5be0-118">Permission type</span></span>                        | <span data-ttu-id="e5be0-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5be0-119">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5be0-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5be0-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5be0-121">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5be0-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="e5be0-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5be0-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5be0-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5be0-123">Not supported.</span></span> |
| <span data-ttu-id="e5be0-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5be0-124">Application</span></span>                            | <span data-ttu-id="e5be0-125">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5be0-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5be0-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5be0-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="e5be0-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5be0-127">Request headers</span></span>

| <span data-ttu-id="e5be0-128">名称</span><span class="sxs-lookup"><span data-stu-id="e5be0-128">Name</span></span>      |<span data-ttu-id="e5be0-129">说明</span><span class="sxs-lookup"><span data-stu-id="e5be0-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5be0-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5be0-130">Authorization</span></span> | <span data-ttu-id="e5be0-131">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e5be0-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5be0-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5be0-132">Request body</span></span>

<span data-ttu-id="e5be0-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5be0-133">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5be0-134">响应</span><span class="sxs-lookup"><span data-stu-id="e5be0-134">Response</span></span>

<span data-ttu-id="e5be0-135">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationOutcome](../resources/educationoutcome.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e5be0-135">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5be0-136">示例</span><span class="sxs-lookup"><span data-stu-id="e5be0-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5be0-137">请求</span><span class="sxs-lookup"><span data-stu-id="e5be0-137">Request</span></span>

<span data-ttu-id="e5be0-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5be0-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5be0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5be0-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes
```
# <a name="c"></a>[<span data-ttu-id="e5be0-140">C#</span><span class="sxs-lookup"><span data-stu-id="e5be0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outcomes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5be0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5be0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outcomes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5be0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5be0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outcomes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5be0-143">Java</span><span class="sxs-lookup"><span data-stu-id="e5be0-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outcomes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5be0-144">响应</span><span class="sxs-lookup"><span data-stu-id="e5be0-144">Response</span></span>

<span data-ttu-id="e5be0-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5be0-145">The following is an example of the response.</span></span>

> <span data-ttu-id="e5be0-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5be0-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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


