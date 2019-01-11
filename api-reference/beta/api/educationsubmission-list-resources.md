---
title: 列表资源
description: 列出与此提交关联的资源。 **SubmissionResource**对象是正在从事实际资源对象学生的包装。 如果这复制从分配过程的工作分配，包装还包括指向上工作分配的资源的指针。 这些资源是工作分配的工作副本。 **SubmittedResources**是正式已提交以进行评分的资源。
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: d7476144159a8f2bd6c4600fe5a2eb80076bc7f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843979"
---
# <a name="list-resources"></a><span data-ttu-id="1cc78-107">列表资源</span><span class="sxs-lookup"><span data-stu-id="1cc78-107">List resources</span></span>

> <span data-ttu-id="1cc78-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1cc78-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cc78-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1cc78-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cc78-110">列出与此提交关联的资源。</span><span class="sxs-lookup"><span data-stu-id="1cc78-110">List the resources associated with this submission.</span></span> <span data-ttu-id="1cc78-111">**SubmissionResource**对象是正在从事实际资源对象学生的包装。</span><span class="sxs-lookup"><span data-stu-id="1cc78-111">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="1cc78-112">如果这复制从分配过程的工作分配，包装还包括指向上工作分配的资源的指针。</span><span class="sxs-lookup"><span data-stu-id="1cc78-112">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="1cc78-113">这些资源是工作分配的工作副本。</span><span class="sxs-lookup"><span data-stu-id="1cc78-113">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="1cc78-114">**SubmittedResources**是正式已提交以进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="1cc78-114">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc78-115">权限</span><span class="sxs-lookup"><span data-stu-id="1cc78-115">Permissions</span></span>
<span data-ttu-id="1cc78-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1cc78-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cc78-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cc78-118">Permission type</span></span>      | <span data-ttu-id="1cc78-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1cc78-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cc78-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cc78-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="1cc78-121">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cc78-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1cc78-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cc78-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc78-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cc78-123">Not supported.</span></span>   |
|<span data-ttu-id="1cc78-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cc78-124">Application</span></span> | <span data-ttu-id="1cc78-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cc78-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1cc78-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cc78-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1cc78-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1cc78-127">Optional query parameters</span></span>
<span data-ttu-id="1cc78-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1cc78-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cc78-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cc78-129">Request headers</span></span>
| <span data-ttu-id="1cc78-130">标头</span><span class="sxs-lookup"><span data-stu-id="1cc78-130">Header</span></span>       | <span data-ttu-id="1cc78-131">值</span><span class="sxs-lookup"><span data-stu-id="1cc78-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1cc78-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cc78-132">Authorization</span></span>  | <span data-ttu-id="1cc78-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1cc78-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1cc78-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cc78-135">Request body</span></span>
<span data-ttu-id="1cc78-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1cc78-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1cc78-137">响应</span><span class="sxs-lookup"><span data-stu-id="1cc78-137">Response</span></span>
<span data-ttu-id="1cc78-138">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSubmissionResource](../resources/educationsubmissionresource.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1cc78-138">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1cc78-139">示例</span><span class="sxs-lookup"><span data-stu-id="1cc78-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cc78-140">请求</span><span class="sxs-lookup"><span data-stu-id="1cc78-140">Request</span></span>
<span data-ttu-id="1cc78-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1cc78-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="1cc78-142">响应</span><span class="sxs-lookup"><span data-stu-id="1cc78-142">Response</span></span>
<span data-ttu-id="1cc78-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1cc78-143">The following is an example of the response.</span></span> 

><span data-ttu-id="1cc78-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1cc78-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
