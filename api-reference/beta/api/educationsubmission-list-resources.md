---
title: 列出资源
description: 列出与此提交相关联的资源。 **SubmissionResource**对象是学生正在处理的实际资源对象周围的包装。 包装还包括指向工作分配中的资源的指针（如果这是在分配过程中从分配中复制的）。 这些资源是工作分配的工作副本。 **SubmittedResources**是已提交以进行评分的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7eb873868cdfc76e29d814e58cd27dfaf53a9917
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007233"
---
# <a name="list-resources"></a><span data-ttu-id="b5d39-107">列出资源</span><span class="sxs-lookup"><span data-stu-id="b5d39-107">List resources</span></span>

<span data-ttu-id="b5d39-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5d39-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5d39-109">列出与此提交相关联的资源。</span><span class="sxs-lookup"><span data-stu-id="b5d39-109">List the resources associated with this submission.</span></span> <span data-ttu-id="b5d39-110">**SubmissionResource**对象是学生正在处理的实际资源对象周围的包装。</span><span class="sxs-lookup"><span data-stu-id="b5d39-110">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="b5d39-111">包装还包括指向工作分配中的资源的指针（如果这是在分配过程中从分配中复制的）。</span><span class="sxs-lookup"><span data-stu-id="b5d39-111">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="b5d39-112">这些资源是工作分配的工作副本。</span><span class="sxs-lookup"><span data-stu-id="b5d39-112">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="b5d39-113">**SubmittedResources**是已提交以进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="b5d39-113">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5d39-114">权限</span><span class="sxs-lookup"><span data-stu-id="b5d39-114">Permissions</span></span>

<span data-ttu-id="b5d39-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5d39-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5d39-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5d39-117">Permission type</span></span>                        | <span data-ttu-id="b5d39-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5d39-118">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b5d39-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5d39-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5d39-120">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="b5d39-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="b5d39-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5d39-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5d39-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5d39-122">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="b5d39-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5d39-123">Application</span></span>                            | <span data-ttu-id="b5d39-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5d39-124">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="b5d39-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5d39-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5d39-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5d39-126">Optional query parameters</span></span>

<span data-ttu-id="b5d39-127">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5d39-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5d39-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5d39-128">Request headers</span></span>

| <span data-ttu-id="b5d39-129">标头</span><span class="sxs-lookup"><span data-stu-id="b5d39-129">Header</span></span>        | <span data-ttu-id="b5d39-130">值</span><span class="sxs-lookup"><span data-stu-id="b5d39-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="b5d39-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5d39-131">Authorization</span></span> | <span data-ttu-id="b5d39-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5d39-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5d39-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5d39-134">Request body</span></span>

<span data-ttu-id="b5d39-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5d39-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5d39-136">响应</span><span class="sxs-lookup"><span data-stu-id="b5d39-136">Response</span></span>

<span data-ttu-id="b5d39-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b5d39-137">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5d39-138">示例</span><span class="sxs-lookup"><span data-stu-id="b5d39-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5d39-139">请求</span><span class="sxs-lookup"><span data-stu-id="b5d39-139">Request</span></span>

<span data-ttu-id="b5d39-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b5d39-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

##### <a name="response"></a><span data-ttu-id="b5d39-141">响应</span><span class="sxs-lookup"><span data-stu-id="b5d39-141">Response</span></span>

<span data-ttu-id="b5d39-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5d39-142">The following is an example of the response.</span></span> 

><span data-ttu-id="b5d39-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b5d39-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


