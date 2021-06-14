---
title: 更新 educationOutcome
description: 更新 educationOutcome 对象的属性。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6b3fba4f87f17528c1e4774b34ba4faeae43bfb
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912286"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="b9de9-103">更新 educationoutcome</span><span class="sxs-lookup"><span data-stu-id="b9de9-103">Update educationoutcome</span></span>

<span data-ttu-id="b9de9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9de9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9de9-105">更新 [educationOutcome 对象](../resources/educationoutcome.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b9de9-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9de9-106">权限</span><span class="sxs-lookup"><span data-stu-id="b9de9-106">Permissions</span></span>

<span data-ttu-id="b9de9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9de9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9de9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9de9-109">Permission type</span></span>                        | <span data-ttu-id="b9de9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9de9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9de9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9de9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9de9-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9de9-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="b9de9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9de9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9de9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9de9-114">Not supported.</span></span> |
| <span data-ttu-id="b9de9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9de9-115">Application</span></span>                            | <span data-ttu-id="b9de9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9de9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9de9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9de9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
```

## <a name="request-headers"></a><span data-ttu-id="b9de9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9de9-118">Request headers</span></span>

| <span data-ttu-id="b9de9-119">名称</span><span class="sxs-lookup"><span data-stu-id="b9de9-119">Name</span></span>       | <span data-ttu-id="b9de9-120">说明</span><span class="sxs-lookup"><span data-stu-id="b9de9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b9de9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9de9-121">Authorization</span></span> | <span data-ttu-id="b9de9-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b9de9-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9de9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9de9-123">Request body</span></span>

<span data-ttu-id="b9de9-124">在请求正文中，仅提供要更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="b9de9-124">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="b9de9-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b9de9-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b9de9-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b9de9-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="b9de9-127">educationOutcome 对象将为以下派生类型之一 **：educationPointsOutcome、educationFeedbackOutcome** 或 **educationRubricOutcome**。 </span><span class="sxs-lookup"><span data-stu-id="b9de9-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="b9de9-128">提供与要修补的结果类型相关的特定属性。</span><span class="sxs-lookup"><span data-stu-id="b9de9-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="b9de9-129">所有派生的结果类型都有一个适合该结果类型的常规和"已发布"属性;例如 **，points** 和 **publishedPoints** **、feedback** 和 **publishedFeedback**。</span><span class="sxs-lookup"><span data-stu-id="b9de9-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="b9de9-130">不要更新"published"属性;供内部使用。</span><span class="sxs-lookup"><span data-stu-id="b9de9-130">Don't update the "published" property; it is for internal use.</span></span> <span data-ttu-id="b9de9-131">例如，若要向 **educationPointsOutcome** 分配点，请更新 **points** 属性，但不更新 **publishedPoint。**</span><span class="sxs-lookup"><span data-stu-id="b9de9-131">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but Don't update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="b9de9-132">响应</span><span class="sxs-lookup"><span data-stu-id="b9de9-132">Response</span></span>

<span data-ttu-id="b9de9-133">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationOutcome](../resources/educationoutcome.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9de9-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9de9-134">示例</span><span class="sxs-lookup"><span data-stu-id="b9de9-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="b9de9-135">示例 1：更新反馈结果</span><span class="sxs-lookup"><span data-stu-id="b9de9-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="b9de9-136">请求</span><span class="sxs-lookup"><span data-stu-id="b9de9-136">Request</span></span>

<span data-ttu-id="b9de9-137">下面是请求更新反馈结果的示例。</span><span class="sxs-lookup"><span data-stu-id="b9de9-137">The following is an example of the request for updating a feedback outcome.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
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

#### <a name="response"></a><span data-ttu-id="b9de9-138">响应</span><span class="sxs-lookup"><span data-stu-id="b9de9-138">Response</span></span>

<span data-ttu-id="b9de9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9de9-139">The following is an example of the response.</span></span>

> <span data-ttu-id="b9de9-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9de9-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="b9de9-141">示例 2：更新点结果</span><span class="sxs-lookup"><span data-stu-id="b9de9-141">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="b9de9-142">请求</span><span class="sxs-lookup"><span data-stu-id="b9de9-142">Request</span></span>

<span data-ttu-id="b9de9-143">下面是请求更新点结果的示例。</span><span class="sxs-lookup"><span data-stu-id="b9de9-143">The following is an example of the request for updating a points outcome.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "points":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGrade",
        "points":85.0
    }
}
```

#### <a name="response"></a><span data-ttu-id="b9de9-144">响应</span><span class="sxs-lookup"><span data-stu-id="b9de9-144">Response</span></span>

<span data-ttu-id="b9de9-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9de9-145">The following is an example of the response.</span></span>

> <span data-ttu-id="b9de9-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9de9-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="b9de9-147">示例 3：更新评估结果</span><span class="sxs-lookup"><span data-stu-id="b9de9-147">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="b9de9-148">请求</span><span class="sxs-lookup"><span data-stu-id="b9de9-148">Request</span></span>

<span data-ttu-id="b9de9-149">下面是一个请求更新评估结果的示例。</span><span class="sxs-lookup"><span data-stu-id="b9de9-149">The following is an example of the request for updating a rubric outcome.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
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

#### <a name="response"></a><span data-ttu-id="b9de9-150">响应</span><span class="sxs-lookup"><span data-stu-id="b9de9-150">Response</span></span>

<span data-ttu-id="b9de9-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9de9-151">The following is an example of the response.</span></span>

> <span data-ttu-id="b9de9-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9de9-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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


