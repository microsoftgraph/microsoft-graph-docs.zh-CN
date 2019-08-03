---
title: 更新 educationOutcome
description: 更新 educationOutcome 对象的属性。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2c7b85d3456927e6a63f61f11722dfe8eccf270e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173179"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="16fe6-103">更新 educationoutcome</span><span class="sxs-lookup"><span data-stu-id="16fe6-103">Update educationoutcome</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16fe6-104">更新[educationOutcome](../resources/educationoutcome.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="16fe6-104">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16fe6-105">权限</span><span class="sxs-lookup"><span data-stu-id="16fe6-105">Permissions</span></span>

<span data-ttu-id="16fe6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16fe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16fe6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="16fe6-108">Permission type</span></span>                        | <span data-ttu-id="16fe6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16fe6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="16fe6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16fe6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="16fe6-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="16fe6-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="16fe6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16fe6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16fe6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="16fe6-113">Not supported.</span></span> |
| <span data-ttu-id="16fe6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="16fe6-114">Application</span></span>                            | <span data-ttu-id="16fe6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="16fe6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16fe6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16fe6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="16fe6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="16fe6-117">Request headers</span></span>

| <span data-ttu-id="16fe6-118">名称</span><span class="sxs-lookup"><span data-stu-id="16fe6-118">Name</span></span>       | <span data-ttu-id="16fe6-119">说明</span><span class="sxs-lookup"><span data-stu-id="16fe6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="16fe6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="16fe6-120">Authorization</span></span> | <span data-ttu-id="16fe6-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="16fe6-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="16fe6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="16fe6-122">Request body</span></span>

<span data-ttu-id="16fe6-123">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="16fe6-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="16fe6-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="16fe6-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="16fe6-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="16fe6-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="16fe6-126">EducationOutcome 对象将为以下派生类型之一: **educationPointsOutcome**、 **educationFeedbackOutcome**或**educationRubricOutcome**。</span><span class="sxs-lookup"><span data-stu-id="16fe6-126">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="16fe6-127">提供与要修补的结果类型相关的特定属性。</span><span class="sxs-lookup"><span data-stu-id="16fe6-127">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="16fe6-128">所有派生结果类型都有一个与该结果类型相对应的常规和 "已发布" 属性;例如,**点**和**publishedPoints**、**反馈**和**publishedFeedback**。</span><span class="sxs-lookup"><span data-stu-id="16fe6-128">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="16fe6-129">不更新 "已发布" 属性;它仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="16fe6-129">Do not update the "published" property; it is for internal use.</span></span> <span data-ttu-id="16fe6-130">例如, 若要向**educationPointsOutcome**分配点, 请更新**points**属性, 但不要更新**publishedPoints**。</span><span class="sxs-lookup"><span data-stu-id="16fe6-130">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but do not update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="16fe6-131">响应</span><span class="sxs-lookup"><span data-stu-id="16fe6-131">Response</span></span>

<span data-ttu-id="16fe6-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[educationOutcome](../resources/educationoutcome.md)对象。</span><span class="sxs-lookup"><span data-stu-id="16fe6-132">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16fe6-133">示例</span><span class="sxs-lookup"><span data-stu-id="16fe6-133">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="16fe6-134">示例 1: 更新反馈结果</span><span class="sxs-lookup"><span data-stu-id="16fe6-134">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="16fe6-135">请求</span><span class="sxs-lookup"><span data-stu-id="16fe6-135">Request</span></span>

<span data-ttu-id="16fe6-136">下面是更新反馈结果的请求示例。</span><span class="sxs-lookup"><span data-stu-id="16fe6-136">The following is an example of the request for updating a feedback outcome.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationFeedbackOutcome",
    "feedback":{
        "text":{
            "content":"This is feedback for the assignment as a whole.",
            "contentType":"text"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="16fe6-137">响应</span><span class="sxs-lookup"><span data-stu-id="16fe6-137">Response</span></span>

<span data-ttu-id="16fe6-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16fe6-138">The following is an example of the response.</span></span>

> <span data-ttu-id="16fe6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="16fe6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFeedbackOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
    "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
    "lastModifiedBy": {
        "user": {
            "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "feedback": {
        "feedbackDateTime": "2019-07-31T21:10:30.3231461Z",
        "text": {
            "content": "This is feedback for the assignment as a whole.",
            "contentType": "text"
        },
        "feedbackBy": {
            "user": {
                "id": "9391878d-903c-406c-bb1c-0f17d00fd878",
            }
        }
    }
}
```

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="16fe6-141">示例 2: 更新点结果</span><span class="sxs-lookup"><span data-stu-id="16fe6-141">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="16fe6-142">请求</span><span class="sxs-lookup"><span data-stu-id="16fe6-142">Request</span></span>

<span data-ttu-id="16fe6-143">下面是更新点结果的请求示例。</span><span class="sxs-lookup"><span data-stu-id="16fe6-143">The following is an example of the request for updating a points outcome.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "points":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGrade",
        "points":85.0
    }
}
```

#### <a name="response"></a><span data-ttu-id="16fe6-144">响应</span><span class="sxs-lookup"><span data-stu-id="16fe6-144">Response</span></span>

<span data-ttu-id="16fe6-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16fe6-145">The following is an example of the response.</span></span>

> <span data-ttu-id="16fe6-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="16fe6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "id":"ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
    "lastModifiedBy":{
        "user":{
            "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "points":{
        "gradedDateTime":"2019-07-15T22:35:48.2429387Z",
        "points":85.0,
        "gradedBy":{
            "user":{
                "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
            }
        }
    }
}
```

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="16fe6-148">示例 3: 更新 Rubric 结果</span><span class="sxs-lookup"><span data-stu-id="16fe6-148">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="16fe6-149">请求</span><span class="sxs-lookup"><span data-stu-id="16fe6-149">Request</span></span>

<span data-ttu-id="16fe6-150">下面是更新 rubric 结果的请求示例。</span><span class="sxs-lookup"><span data-stu-id="16fe6-150">The following is an example of the request for updating a rubric outcome.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationRubricOutcome",
    "rubricQualityFeedback":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback":{
                "content":"This is feedback specific to the first quality of the rubric.",
                "contentType":"text"
            }
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback":{
                "content":"This is feedback specific to the second quality of the rubric.",
                "contentType":"text"
            }
        }
    ],
    "rubricQualitySelectedLevels":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId":"4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId":"aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="16fe6-151">响应</span><span class="sxs-lookup"><span data-stu-id="16fe6-151">Response</span></span>

<span data-ttu-id="16fe6-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16fe6-152">The following is an example of the response.</span></span>

> <span data-ttu-id="16fe6-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="16fe6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.type": "#microsoft.graph.educationRubricOutcome",
    "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
    "rubricQualityFeedback": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback": {
                "content": "This is feedback specific to the first quality of the rubric.",
                "contentType": "text"
            }
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback": {
                "content": "This is feedback specific to the second quality of the rubric.",
                "contentType": "text"
            }
        }
    ],
    "rubricQualitySelectedLevels": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId": "4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId": "aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationoutcome",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
