---
title: 列出 submittedResources
description: 列出已提交进行评分的资源。 拥有提交的学生无法在不重新提交工作分配的情况下更改已提交的列表。 这是围绕真实资源的包装, 如果此资源是从工作分配复制的, 则可以包含指向实际工作分配资源的指针。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fa98baff82250e8da68f21c2b3779b387977f763
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325178"
---
# <a name="list-submittedresources"></a><span data-ttu-id="26d8a-105">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="26d8a-105">List submittedResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26d8a-106">列出已提交进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="26d8a-106">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="26d8a-107">拥有提交的学生无法在不重新提交工作分配的情况下更改已提交的列表。</span><span class="sxs-lookup"><span data-stu-id="26d8a-107">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="26d8a-108">这是围绕真实资源的包装, 如果此资源是从工作分配复制的, 则可以包含指向实际工作分配资源的指针。</span><span class="sxs-lookup"><span data-stu-id="26d8a-108">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="26d8a-109">权限</span><span class="sxs-lookup"><span data-stu-id="26d8a-109">Permissions</span></span>
<span data-ttu-id="26d8a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26d8a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26d8a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="26d8a-112">Permission type</span></span>      | <span data-ttu-id="26d8a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26d8a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26d8a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26d8a-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="26d8a-115">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="26d8a-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="26d8a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26d8a-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="26d8a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="26d8a-117">Not supported.</span></span>  |
|<span data-ttu-id="26d8a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="26d8a-118">Application</span></span> | <span data-ttu-id="26d8a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="26d8a-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="26d8a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26d8a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="26d8a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="26d8a-121">Optional query parameters</span></span>
<span data-ttu-id="26d8a-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="26d8a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26d8a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="26d8a-123">Request headers</span></span>
| <span data-ttu-id="26d8a-124">标头</span><span class="sxs-lookup"><span data-stu-id="26d8a-124">Header</span></span>       | <span data-ttu-id="26d8a-125">值</span><span class="sxs-lookup"><span data-stu-id="26d8a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26d8a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="26d8a-126">Authorization</span></span>  | <span data-ttu-id="26d8a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26d8a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26d8a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="26d8a-129">Request body</span></span>
<span data-ttu-id="26d8a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26d8a-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="26d8a-131">响应</span><span class="sxs-lookup"><span data-stu-id="26d8a-131">Response</span></span>
<span data-ttu-id="26d8a-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSubmissionResource](../resources/educationsubmissionresource.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="26d8a-132">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26d8a-133">示例</span><span class="sxs-lookup"><span data-stu-id="26d8a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26d8a-134">请求</span><span class="sxs-lookup"><span data-stu-id="26d8a-134">Request</span></span>
<span data-ttu-id="26d8a-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26d8a-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="26d8a-136">响应</span><span class="sxs-lookup"><span data-stu-id="26d8a-136">Response</span></span>
<span data-ttu-id="26d8a-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26d8a-137">The following is an example of the response.</span></span> 

><span data-ttu-id="26d8a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26d8a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource",
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
        "link": "https://www.microsoft.com
        },
        "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource" 
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
