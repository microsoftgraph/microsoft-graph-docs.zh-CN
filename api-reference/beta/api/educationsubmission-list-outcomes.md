---
title: 列表结果
description: 检索 educationoutcome 对象的列表。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c8837d1edffc09e842f4885c9b48f262749a85ee
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460970"
---
# <a name="list-outcomes"></a><span data-ttu-id="48850-103">列表结果</span><span class="sxs-lookup"><span data-stu-id="48850-103">List outcomes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48850-104">检索[educationOutcome](../resources/educationoutcome.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="48850-104">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="48850-105">有三种类型的结果: **educationPointsOutcome**、 **educationFeedbackOutcome**和**educationRubricOutcome**。</span><span class="sxs-lookup"><span data-stu-id="48850-105">There are three types of outcomes: **educationPointsOutcome**, **educationFeedbackOutcome**, and **educationRubricOutcome**.</span></span>

<span data-ttu-id="48850-106">对信用卡分配 (没有点值, 没有 rubric 的人) 的提交将具有[educationFeedbackOutcome](../resources/educationpointsoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="48850-106">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="48850-107">(它可能还会返回[educationPointsOutcome](../resources/educationpointsoutcome.md), 但忽略该结果。)</span><span class="sxs-lookup"><span data-stu-id="48850-107">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="48850-108">为 "点" 分配 (分配了 "点" 值) 进行提交时, 将同时具有[educationFeedbackOutcome](../resources/educationpointsoutcome.md)和[educationPointsOutcome](../resources/educationpointsoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="48850-108">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="48850-109">包含附加 rubric 的工作分配的提交, 如果 rubric 是信用 rubric (没有点), 将具有[educationFeedbackOutcome](../resources/educationpointsoutcome.md)和[educationRubricOutcome](../resources/educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="48850-109">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="48850-110">(它可能还会返回[educationPointsOutcome](../resources/educationpointsoutcome.md), 但忽略该结果。)</span><span class="sxs-lookup"><span data-stu-id="48850-110">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="48850-111">提交包含附加 rubric 的工作分配, 如果 rubric 是一个点 rubric, 则会有一个[educationFeedbackOutcome](../resources/educationpointsoutcome.md), [educationPointsOutcome] (.。。/resources/educationpointsoutcome.md 和[educationRubricOutcome](../resources/educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="48850-111">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="48850-112">所有结果类型都具有与该结果类型相对应的常规和已发布属性;例如,**点**和**publishedPoints**、**反馈**和**publishedFeedback**。</span><span class="sxs-lookup"><span data-stu-id="48850-112">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="48850-113">常规属性是教师更新的最新值;已发布的属性是返回给学生的最新值。</span><span class="sxs-lookup"><span data-stu-id="48850-113">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="48850-114">权限</span><span class="sxs-lookup"><span data-stu-id="48850-114">Permissions</span></span>

<span data-ttu-id="48850-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48850-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48850-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="48850-117">Permission type</span></span>                        | <span data-ttu-id="48850-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48850-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48850-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48850-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="48850-120">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="48850-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="48850-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48850-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48850-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="48850-122">Not supported.</span></span> |
| <span data-ttu-id="48850-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="48850-123">Application</span></span>                            | <span data-ttu-id="48850-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="48850-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48850-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48850-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="48850-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="48850-126">Request headers</span></span>

| <span data-ttu-id="48850-127">名称</span><span class="sxs-lookup"><span data-stu-id="48850-127">Name</span></span>      |<span data-ttu-id="48850-128">说明</span><span class="sxs-lookup"><span data-stu-id="48850-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48850-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="48850-129">Authorization</span></span> | <span data-ttu-id="48850-130">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="48850-130">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="48850-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="48850-131">Request body</span></span>

<span data-ttu-id="48850-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48850-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48850-133">响应</span><span class="sxs-lookup"><span data-stu-id="48850-133">Response</span></span>

<span data-ttu-id="48850-134">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationOutcome](../resources/educationoutcome.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="48850-134">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48850-135">示例</span><span class="sxs-lookup"><span data-stu-id="48850-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48850-136">请求</span><span class="sxs-lookup"><span data-stu-id="48850-136">Request</span></span>

<span data-ttu-id="48850-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48850-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48850-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="48850-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48850-139">C#</span><span class="sxs-lookup"><span data-stu-id="48850-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outcomes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48850-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48850-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outcomes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48850-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="48850-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outcomes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48850-142">响应</span><span class="sxs-lookup"><span data-stu-id="48850-142">Response</span></span>

<span data-ttu-id="48850-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48850-143">The following is an example of the response.</span></span>

> <span data-ttu-id="48850-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="48850-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
