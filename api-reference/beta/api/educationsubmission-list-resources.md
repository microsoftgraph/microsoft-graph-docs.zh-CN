---
title: 列出资源
description: 列出与此提交相关联的资源。 **SubmissionResource**对象是学生正在处理的实际资源对象周围的包装。 包装还包括指向工作分配中的资源的指针 (如果这是在分配过程中从分配中复制的)。 这些资源是工作分配的工作副本。 **SubmittedResources**是已提交以进行评分的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 51a70d3554ea0dac3c5e3487bb9f9dab88addba2
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34749966"
---
# <a name="list-resources"></a><span data-ttu-id="cf2cb-107">列出资源</span><span class="sxs-lookup"><span data-stu-id="cf2cb-107">List resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf2cb-108">列出与此提交相关联的资源。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-108">List the resources associated with this submission.</span></span> <span data-ttu-id="cf2cb-109">**SubmissionResource**对象是学生正在处理的实际资源对象周围的包装。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-109">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="cf2cb-110">包装还包括指向工作分配中的资源的指针 (如果这是在分配过程中从分配中复制的)。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-110">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="cf2cb-111">这些资源是工作分配的工作副本。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-111">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="cf2cb-112">**SubmittedResources**是已提交以进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-112">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf2cb-113">权限</span><span class="sxs-lookup"><span data-stu-id="cf2cb-113">Permissions</span></span>

<span data-ttu-id="cf2cb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf2cb-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf2cb-116">Permission type</span></span>                        | <span data-ttu-id="cf2cb-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf2cb-117">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cf2cb-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf2cb-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf2cb-119">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="cf2cb-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="cf2cb-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf2cb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf2cb-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-121">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="cf2cb-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf2cb-122">Application</span></span>                            | <span data-ttu-id="cf2cb-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-123">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="cf2cb-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf2cb-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf2cb-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf2cb-125">Optional query parameters</span></span>

<span data-ttu-id="cf2cb-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf2cb-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf2cb-127">Request headers</span></span>

| <span data-ttu-id="cf2cb-128">标头</span><span class="sxs-lookup"><span data-stu-id="cf2cb-128">Header</span></span>        | <span data-ttu-id="cf2cb-129">值</span><span class="sxs-lookup"><span data-stu-id="cf2cb-129">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="cf2cb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf2cb-130">Authorization</span></span> | <span data-ttu-id="cf2cb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf2cb-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf2cb-133">Request body</span></span>

<span data-ttu-id="cf2cb-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf2cb-135">响应</span><span class="sxs-lookup"><span data-stu-id="cf2cb-135">Response</span></span>

<span data-ttu-id="cf2cb-136">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSubmissionResource](../resources/educationsubmissionresource.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-136">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf2cb-137">示例</span><span class="sxs-lookup"><span data-stu-id="cf2cb-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf2cb-138">请求</span><span class="sxs-lookup"><span data-stu-id="cf2cb-138">Request</span></span>

<span data-ttu-id="cf2cb-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

##### <a name="response"></a><span data-ttu-id="cf2cb-140">响应</span><span class="sxs-lookup"><span data-stu-id="cf2cb-140">Response</span></span>

<span data-ttu-id="cf2cb-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-141">The following is an example of the response.</span></span> 

><span data-ttu-id="cf2cb-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cf2cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
