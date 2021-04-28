---
title: 列出 submittedResources
description: 列出已正式提交进行评分的资源。 拥有提交的学生如果不重新提交作业，则无法更改提交的列表。 这是实际资源的包装器，如果此资源是从工作分配复制的，则可以包含一个返回实际工作分配资源的指针。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 861ee3371517d95e89c9077d6e139202d370a917
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061838"
---
# <a name="list-submittedresources"></a><span data-ttu-id="2c92f-105">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="2c92f-105">List submittedResources</span></span>

<span data-ttu-id="2c92f-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c92f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c92f-107">列出已正式提交进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="2c92f-107">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="2c92f-108">拥有提交的学生如果不重新提交作业，则无法更改提交的列表。</span><span class="sxs-lookup"><span data-stu-id="2c92f-108">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="2c92f-109">这是实际资源的包装器，如果此资源是从工作分配复制的，则可以包含一个返回实际工作分配资源的指针。</span><span class="sxs-lookup"><span data-stu-id="2c92f-109">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c92f-110">权限</span><span class="sxs-lookup"><span data-stu-id="2c92f-110">Permissions</span></span>
<span data-ttu-id="2c92f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c92f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c92f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c92f-113">Permission type</span></span>      | <span data-ttu-id="2c92f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c92f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c92f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c92f-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="2c92f-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c92f-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2c92f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c92f-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2c92f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c92f-118">Not supported.</span></span>  |
|<span data-ttu-id="2c92f-119">Application\*</span><span class="sxs-lookup"><span data-stu-id="2c92f-119">Application\*</span></span> | <span data-ttu-id="2c92f-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c92f-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="2c92f-121">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="2c92f-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="2c92f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c92f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2c92f-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c92f-123">Optional query parameters</span></span>
<span data-ttu-id="2c92f-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c92f-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c92f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c92f-125">Request headers</span></span>
| <span data-ttu-id="2c92f-126">标头</span><span class="sxs-lookup"><span data-stu-id="2c92f-126">Header</span></span>       | <span data-ttu-id="2c92f-127">值</span><span class="sxs-lookup"><span data-stu-id="2c92f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c92f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c92f-128">Authorization</span></span>  | <span data-ttu-id="2c92f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c92f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c92f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c92f-131">Request body</span></span>
<span data-ttu-id="2c92f-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c92f-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2c92f-133">响应</span><span class="sxs-lookup"><span data-stu-id="2c92f-133">Response</span></span>
<span data-ttu-id="2c92f-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c92f-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c92f-135">示例</span><span class="sxs-lookup"><span data-stu-id="2c92f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c92f-136">请求</span><span class="sxs-lookup"><span data-stu-id="2c92f-136">Request</span></span>
<span data-ttu-id="2c92f-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c92f-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="2c92f-138">响应</span><span class="sxs-lookup"><span data-stu-id="2c92f-138">Response</span></span>
<span data-ttu-id="2c92f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c92f-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2c92f-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2c92f-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
