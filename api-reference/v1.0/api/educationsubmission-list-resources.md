---
title: 列出提交资源
description: 列出与提交关联的资源。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2d291ac67988d3960c70df1f8183b0c8989ce008
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911419"
---
# <a name="list-submission-resources"></a><span data-ttu-id="13746-103">列出提交资源</span><span class="sxs-lookup"><span data-stu-id="13746-103">List submission resources</span></span>

<span data-ttu-id="13746-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13746-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13746-105">列出与提交关联的 [资源](../resources/educationsubmission.md)。</span><span class="sxs-lookup"><span data-stu-id="13746-105">List the resources associated with a [submission](../resources/educationsubmission.md).</span></span> 

<span data-ttu-id="13746-106">**submissionResource** 对象是学生正在处理的实际资源对象的包装。</span><span class="sxs-lookup"><span data-stu-id="13746-106">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="13746-107">如果资源是在分配过程中从分配复制的，包装器还包括指向分配上的资源的指针。</span><span class="sxs-lookup"><span data-stu-id="13746-107">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="13746-108">这些资源是工作分配的工作副本。</span><span class="sxs-lookup"><span data-stu-id="13746-108">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="13746-109">**submittedResources** 是已正式提交进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="13746-109">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="13746-110">权限</span><span class="sxs-lookup"><span data-stu-id="13746-110">Permissions</span></span>

<span data-ttu-id="13746-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13746-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="13746-113">Permission type</span></span>                        | <span data-ttu-id="13746-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13746-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="13746-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13746-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="13746-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13746-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="13746-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13746-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13746-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="13746-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="13746-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="13746-119">Application</span></span>                            | <span data-ttu-id="13746-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13746-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13746-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13746-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13746-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="13746-122">Optional query parameters</span></span>

<span data-ttu-id="13746-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13746-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13746-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="13746-124">Request headers</span></span>

| <span data-ttu-id="13746-125">标头</span><span class="sxs-lookup"><span data-stu-id="13746-125">Header</span></span>        | <span data-ttu-id="13746-126">值</span><span class="sxs-lookup"><span data-stu-id="13746-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="13746-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="13746-127">Authorization</span></span> | <span data-ttu-id="13746-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13746-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13746-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="13746-130">Request body</span></span>

<span data-ttu-id="13746-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13746-131">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13746-132">响应</span><span class="sxs-lookup"><span data-stu-id="13746-132">Response</span></span>

<span data-ttu-id="13746-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="13746-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13746-134">示例</span><span class="sxs-lookup"><span data-stu-id="13746-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="13746-135">请求</span><span class="sxs-lookup"><span data-stu-id="13746-135">Request</span></span>

<span data-ttu-id="13746-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13746-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```

### <a name="response"></a><span data-ttu-id="13746-137">响应</span><span class="sxs-lookup"><span data-stu-id="13746-137">Response</span></span>

<span data-ttu-id="13746-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13746-138">The following is an example of the response.</span></span> 

><span data-ttu-id="13746-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13746-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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
