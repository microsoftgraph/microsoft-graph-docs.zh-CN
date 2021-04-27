---
title: 列出 submittedResources
description: 列出已正式提交进行评分的资源。 拥有提交的学生如果不重新提交作业，则无法更改提交的列表。 这是实际资源的包装器，如果此资源是从工作分配复制的，则可以包含一个返回实际工作分配资源的指针。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8b8aba382edb61ce54d4c1a036edee9fd9b3c057
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043191"
---
# <a name="list-submittedresources"></a><span data-ttu-id="c62e2-105">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="c62e2-105">List submittedResources</span></span>

<span data-ttu-id="c62e2-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c62e2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c62e2-107">列出已正式提交进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="c62e2-107">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="c62e2-108">拥有提交的学生如果不重新提交作业，则无法更改提交的列表。</span><span class="sxs-lookup"><span data-stu-id="c62e2-108">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="c62e2-109">这是实际资源的包装器，如果此资源是从工作分配复制的，则可以包含一个返回实际工作分配资源的指针。</span><span class="sxs-lookup"><span data-stu-id="c62e2-109">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="c62e2-110">权限</span><span class="sxs-lookup"><span data-stu-id="c62e2-110">Permissions</span></span>
<span data-ttu-id="c62e2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c62e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c62e2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c62e2-113">Permission type</span></span>      | <span data-ttu-id="c62e2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c62e2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c62e2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c62e2-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="c62e2-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c62e2-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c62e2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c62e2-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c62e2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c62e2-118">Not supported.</span></span>  |
|<span data-ttu-id="c62e2-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c62e2-119">Application</span></span> | <span data-ttu-id="c62e2-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c62e2-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c62e2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c62e2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c62e2-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c62e2-122">Optional query parameters</span></span>
<span data-ttu-id="c62e2-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c62e2-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c62e2-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c62e2-124">Request headers</span></span>
| <span data-ttu-id="c62e2-125">标头</span><span class="sxs-lookup"><span data-stu-id="c62e2-125">Header</span></span>       | <span data-ttu-id="c62e2-126">值</span><span class="sxs-lookup"><span data-stu-id="c62e2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c62e2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c62e2-127">Authorization</span></span>  | <span data-ttu-id="c62e2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c62e2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c62e2-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c62e2-130">Request body</span></span>
<span data-ttu-id="c62e2-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c62e2-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c62e2-132">响应</span><span class="sxs-lookup"><span data-stu-id="c62e2-132">Response</span></span>
<span data-ttu-id="c62e2-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c62e2-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c62e2-134">示例</span><span class="sxs-lookup"><span data-stu-id="c62e2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c62e2-135">请求</span><span class="sxs-lookup"><span data-stu-id="c62e2-135">Request</span></span>
<span data-ttu-id="c62e2-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c62e2-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="c62e2-137">响应</span><span class="sxs-lookup"><span data-stu-id="c62e2-137">Response</span></span>
<span data-ttu-id="c62e2-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c62e2-138">The following is an example of the response.</span></span> 

><span data-ttu-id="c62e2-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c62e2-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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
          "link": "https://www.microsoft.com"
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
