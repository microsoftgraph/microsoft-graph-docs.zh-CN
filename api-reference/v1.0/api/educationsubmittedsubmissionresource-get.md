---
title: 获取 educationSubmittedSubmissionResource
description: 检索已提交资源。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00c9bb49c43dd809945166a6dca4a05a76a87b5f
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912343"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="617b5-103">获取 educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="617b5-103">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="617b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="617b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="617b5-105">检索 [已提交资源](../resources/educationsubmissionresource.md)。</span><span class="sxs-lookup"><span data-stu-id="617b5-105">Retrieve a [submitted resource](../resources/educationsubmissionresource.md).</span></span> 

<span data-ttu-id="617b5-106">在学生提交后，教师或具有应用程序权限的应用程序将可以使用此功能，并且将在教师发布提交后提供给学生。</span><span class="sxs-lookup"><span data-stu-id="617b5-106">This will be available to a teacher or an application with application permissions after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="617b5-107">请注意，教师可以在一些资源中留下笔记。</span><span class="sxs-lookup"><span data-stu-id="617b5-107">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="617b5-108">权限</span><span class="sxs-lookup"><span data-stu-id="617b5-108">Permissions</span></span>
<span data-ttu-id="617b5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="617b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="617b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="617b5-111">Permission type</span></span>      | <span data-ttu-id="617b5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="617b5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="617b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="617b5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="617b5-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="617b5-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="617b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="617b5-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="617b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="617b5-116">Not supported.</span></span>  |
|<span data-ttu-id="617b5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="617b5-117">Application</span></span> | <span data-ttu-id="617b5-118">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="617b5-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="617b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="617b5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="617b5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="617b5-120">Optional query parameters</span></span>
<span data-ttu-id="617b5-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="617b5-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="617b5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="617b5-122">Request headers</span></span>
| <span data-ttu-id="617b5-123">标头</span><span class="sxs-lookup"><span data-stu-id="617b5-123">Header</span></span>       | <span data-ttu-id="617b5-124">值</span><span class="sxs-lookup"><span data-stu-id="617b5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="617b5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="617b5-125">Authorization</span></span>  | <span data-ttu-id="617b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="617b5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="617b5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="617b5-128">Request body</span></span>
<span data-ttu-id="617b5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="617b5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="617b5-130">响应</span><span class="sxs-lookup"><span data-stu-id="617b5-130">Response</span></span>
<span data-ttu-id="617b5-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="617b5-131">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span> <span data-ttu-id="617b5-132">否则，返回 `404 Not found` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="617b5-132">Otherwise, returns a `404 Not found` response code.</span></span>

## <a name="example"></a><span data-ttu-id="617b5-133">示例</span><span class="sxs-lookup"><span data-stu-id="617b5-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="617b5-134">请求</span><span class="sxs-lookup"><span data-stu-id="617b5-134">Request</span></span>
<span data-ttu-id="617b5-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="617b5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/f973bc68-2adb-4cf7-8b15-a57a1936b60c/assignments/8b890b42-a1df-478b-bff5-6814afb1afc2/submissions/6d71b348-898a-40cd-8e71-35127eed97f5/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
### <a name="response"></a><span data-ttu-id="617b5-136">响应</span><span class="sxs-lookup"><span data-stu-id="617b5-136">Response</span></span>
<span data-ttu-id="617b5-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="617b5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="617b5-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="617b5-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource"
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
