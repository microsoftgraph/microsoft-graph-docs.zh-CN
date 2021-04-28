---
title: 获取 educationSubmittedSubmissionResource
description: 返回已提交资源。 在学生提交后，教师或具有应用程序权限的应用程序将可以使用此功能，并且将在教师发布提交后提供给学生。  请注意，教师可以在一些资源中留下笔记。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d2ce500e4a6a2dfc7cac779ddf3ab28e28476645
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061845"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="4cca9-105">获取 educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="4cca9-105">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="4cca9-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cca9-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cca9-107">返回已提交资源。</span><span class="sxs-lookup"><span data-stu-id="4cca9-107">Returns a submitted resource.</span></span> <span data-ttu-id="4cca9-108">在学生提交后，教师或具有应用程序权限的应用程序将可以使用此功能，并且将在教师发布提交后提供给学生。</span><span class="sxs-lookup"><span data-stu-id="4cca9-108">This will be available to a teacher or an application with application permissions after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="4cca9-109">请注意，教师可以在一些资源中留下笔记。</span><span class="sxs-lookup"><span data-stu-id="4cca9-109">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cca9-110">权限</span><span class="sxs-lookup"><span data-stu-id="4cca9-110">Permissions</span></span>
<span data-ttu-id="4cca9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cca9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cca9-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cca9-113">Permission type</span></span>      | <span data-ttu-id="4cca9-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cca9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cca9-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cca9-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="4cca9-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cca9-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4cca9-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cca9-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4cca9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cca9-118">Not supported.</span></span>  |
|<span data-ttu-id="4cca9-119">Application\*</span><span class="sxs-lookup"><span data-stu-id="4cca9-119">Application\*</span></span> | <span data-ttu-id="4cca9-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cca9-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="4cca9-121">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="4cca9-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="4cca9-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cca9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4cca9-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4cca9-123">Optional query parameters</span></span>
<span data-ttu-id="4cca9-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4cca9-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cca9-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cca9-125">Request headers</span></span>
| <span data-ttu-id="4cca9-126">标头</span><span class="sxs-lookup"><span data-stu-id="4cca9-126">Header</span></span>       | <span data-ttu-id="4cca9-127">值</span><span class="sxs-lookup"><span data-stu-id="4cca9-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4cca9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cca9-128">Authorization</span></span>  | <span data-ttu-id="4cca9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4cca9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4cca9-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cca9-131">Request body</span></span>
<span data-ttu-id="4cca9-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4cca9-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4cca9-133">响应</span><span class="sxs-lookup"><span data-stu-id="4cca9-133">Response</span></span>
<span data-ttu-id="4cca9-134">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4cca9-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4cca9-135">示例</span><span class="sxs-lookup"><span data-stu-id="4cca9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cca9-136">请求</span><span class="sxs-lookup"><span data-stu-id="4cca9-136">Request</span></span>
<span data-ttu-id="4cca9-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4cca9-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="4cca9-138">响应</span><span class="sxs-lookup"><span data-stu-id="4cca9-138">Response</span></span>
<span data-ttu-id="4cca9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4cca9-139">The following is an example of the response.</span></span> 

><span data-ttu-id="4cca9-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4cca9-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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