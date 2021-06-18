---
title: 更新 educationOutcome
description: 更新 educationOutcome 对象的属性。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fcc9c011b4c23c088f887184891781af2f9f8338
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991287"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="a93e1-103">更新 educationoutcome</span><span class="sxs-lookup"><span data-stu-id="a93e1-103">Update educationoutcome</span></span>

<span data-ttu-id="a93e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a93e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a93e1-105">更新 [educationOutcome 对象](../resources/educationoutcome.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a93e1-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a93e1-106">权限</span><span class="sxs-lookup"><span data-stu-id="a93e1-106">Permissions</span></span>

<span data-ttu-id="a93e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a93e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a93e1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a93e1-109">Permission type</span></span>                        | <span data-ttu-id="a93e1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a93e1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a93e1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a93e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a93e1-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a93e1-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a93e1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a93e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a93e1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a93e1-114">Not supported.</span></span> |
| <span data-ttu-id="a93e1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a93e1-115">Application</span></span>                            | <span data-ttu-id="a93e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a93e1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a93e1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a93e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
```

## <a name="request-headers"></a><span data-ttu-id="a93e1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a93e1-118">Request headers</span></span>

| <span data-ttu-id="a93e1-119">名称</span><span class="sxs-lookup"><span data-stu-id="a93e1-119">Name</span></span>       | <span data-ttu-id="a93e1-120">说明</span><span class="sxs-lookup"><span data-stu-id="a93e1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a93e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a93e1-121">Authorization</span></span> | <span data-ttu-id="a93e1-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a93e1-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a93e1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a93e1-123">Request body</span></span>

<span data-ttu-id="a93e1-124">在请求正文中，仅提供要更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="a93e1-124">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="a93e1-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a93e1-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a93e1-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a93e1-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="a93e1-127">educationOutcome 对象将为以下派生类型之一 **：educationPointsOutcome、educationFeedbackOutcome** 或 **educationRubricOutcome**。 </span><span class="sxs-lookup"><span data-stu-id="a93e1-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="a93e1-128">提供与要修补的结果类型相关的特定属性。</span><span class="sxs-lookup"><span data-stu-id="a93e1-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="a93e1-129">所有派生的结果类型都有一个适合该结果类型的常规和"已发布"属性;例如 **，points** 和 **publishedPoints** **、feedback** 和 **publishedFeedback**。</span><span class="sxs-lookup"><span data-stu-id="a93e1-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="a93e1-130">不要更新"published"属性;供内部使用。</span><span class="sxs-lookup"><span data-stu-id="a93e1-130">Don't update the "published" property; it is for internal use.</span></span> <span data-ttu-id="a93e1-131">例如，若要向 **educationPointsOutcome** 分配点，请更新 **points** 属性，但不更新 **publishedPoint。**</span><span class="sxs-lookup"><span data-stu-id="a93e1-131">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but Don't update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="a93e1-132">响应</span><span class="sxs-lookup"><span data-stu-id="a93e1-132">Response</span></span>

<span data-ttu-id="a93e1-133">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationOutcome](../resources/educationoutcome.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a93e1-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a93e1-134">示例</span><span class="sxs-lookup"><span data-stu-id="a93e1-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="a93e1-135">示例 1：更新反馈结果</span><span class="sxs-lookup"><span data-stu-id="a93e1-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="a93e1-136">请求</span><span class="sxs-lookup"><span data-stu-id="a93e1-136">Request</span></span>

<span data-ttu-id="a93e1-137">下面是请求更新反馈结果的示例。</span><span class="sxs-lookup"><span data-stu-id="a93e1-137">The following is an example of the request for updating a feedback outcome.</span></span>


# <a name="http"></a>[<span data-ttu-id="a93e1-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a93e1-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a93e1-139">C#</span><span class="sxs-lookup"><span data-stu-id="a93e1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationfeedbackoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a93e1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a93e1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationfeedbackoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a93e1-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a93e1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationfeedbackoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a93e1-142">Java</span><span class="sxs-lookup"><span data-stu-id="a93e1-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationfeedbackoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a93e1-143">响应</span><span class="sxs-lookup"><span data-stu-id="a93e1-143">Response</span></span>

<span data-ttu-id="a93e1-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a93e1-144">The following is an example of the response.</span></span>

> <span data-ttu-id="a93e1-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a93e1-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="a93e1-146">示例 2：更新点结果</span><span class="sxs-lookup"><span data-stu-id="a93e1-146">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="a93e1-147">请求</span><span class="sxs-lookup"><span data-stu-id="a93e1-147">Request</span></span>

<span data-ttu-id="a93e1-148">下面是请求更新点结果的示例。</span><span class="sxs-lookup"><span data-stu-id="a93e1-148">The following is an example of the request for updating a points outcome.</span></span>


# <a name="http"></a>[<span data-ttu-id="a93e1-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="a93e1-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a93e1-150">C#</span><span class="sxs-lookup"><span data-stu-id="a93e1-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationpointsoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a93e1-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a93e1-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationpointsoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a93e1-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a93e1-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationpointsoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a93e1-153">Java</span><span class="sxs-lookup"><span data-stu-id="a93e1-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationpointsoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a93e1-154">响应</span><span class="sxs-lookup"><span data-stu-id="a93e1-154">Response</span></span>

<span data-ttu-id="a93e1-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a93e1-155">The following is an example of the response.</span></span>

> <span data-ttu-id="a93e1-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a93e1-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="a93e1-157">示例 3：更新评估结果</span><span class="sxs-lookup"><span data-stu-id="a93e1-157">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="a93e1-158">请求</span><span class="sxs-lookup"><span data-stu-id="a93e1-158">Request</span></span>

<span data-ttu-id="a93e1-159">下面是一个请求更新评估结果的示例。</span><span class="sxs-lookup"><span data-stu-id="a93e1-159">The following is an example of the request for updating a rubric outcome.</span></span>


# <a name="http"></a>[<span data-ttu-id="a93e1-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a93e1-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a93e1-161">C#</span><span class="sxs-lookup"><span data-stu-id="a93e1-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a93e1-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a93e1-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a93e1-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a93e1-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a93e1-164">Java</span><span class="sxs-lookup"><span data-stu-id="a93e1-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a93e1-165">响应</span><span class="sxs-lookup"><span data-stu-id="a93e1-165">Response</span></span>

<span data-ttu-id="a93e1-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a93e1-166">The following is an example of the response.</span></span>

> <span data-ttu-id="a93e1-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a93e1-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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


