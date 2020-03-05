---
title: 获取 educationSubmittedSubmissionResource
description: 返回已提交的资源。 这在学生提交后将对教师可用，并将在教师发布提交后供学生使用。  请注意，教师可以在某些资源中留下笔记。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0e670022a2d8eb87313952e2429b720bd4a535cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424636"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="06559-105">获取 educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="06559-105">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="06559-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="06559-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06559-107">返回已提交的资源。</span><span class="sxs-lookup"><span data-stu-id="06559-107">Returns a submitted resource.</span></span> <span data-ttu-id="06559-108">这在学生提交后将对教师可用，并将在教师发布提交后供学生使用。</span><span class="sxs-lookup"><span data-stu-id="06559-108">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="06559-109">请注意，教师可以在某些资源中留下笔记。</span><span class="sxs-lookup"><span data-stu-id="06559-109">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="06559-110">权限</span><span class="sxs-lookup"><span data-stu-id="06559-110">Permissions</span></span>
<span data-ttu-id="06559-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06559-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06559-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="06559-113">Permission type</span></span>      | <span data-ttu-id="06559-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06559-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06559-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06559-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="06559-116">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="06559-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="06559-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06559-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="06559-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="06559-118">Not supported.</span></span>  |
|<span data-ttu-id="06559-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="06559-119">Application</span></span> | <span data-ttu-id="06559-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="06559-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="06559-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06559-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06559-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="06559-122">Optional query parameters</span></span>
<span data-ttu-id="06559-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="06559-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06559-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="06559-124">Request headers</span></span>
| <span data-ttu-id="06559-125">标头</span><span class="sxs-lookup"><span data-stu-id="06559-125">Header</span></span>       | <span data-ttu-id="06559-126">值</span><span class="sxs-lookup"><span data-stu-id="06559-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06559-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="06559-127">Authorization</span></span>  | <span data-ttu-id="06559-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06559-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06559-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="06559-130">Request body</span></span>
<span data-ttu-id="06559-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06559-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="06559-132">响应</span><span class="sxs-lookup"><span data-stu-id="06559-132">Response</span></span>
<span data-ttu-id="06559-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[educationSubmissionResource](../resources/educationsubmissionresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="06559-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06559-134">示例</span><span class="sxs-lookup"><span data-stu-id="06559-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06559-135">请求</span><span class="sxs-lookup"><span data-stu-id="06559-135">Request</span></span>
<span data-ttu-id="06559-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="06559-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="06559-137">响应</span><span class="sxs-lookup"><span data-stu-id="06559-137">Response</span></span>
<span data-ttu-id="06559-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="06559-138">The following is an example of the response.</span></span> 

><span data-ttu-id="06559-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="06559-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
      "@odata.type": "microsoft.graph.educationResource"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
