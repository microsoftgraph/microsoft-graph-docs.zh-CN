---
title: 创建 educationSubmissionResource
description: 将资源添加到提交资源列表。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7d107b7ceff798875244740ebbe8c7e68322480b
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993405"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="75002-103">创建 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="75002-103">Create educationSubmissionResource</span></span>

<span data-ttu-id="75002-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75002-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75002-105">将资源添加到提交资源列表。</span><span class="sxs-lookup"><span data-stu-id="75002-105">Add a resource to the submission resource list.</span></span> 

<span data-ttu-id="75002-106">此操作仅能由分配了此提交的学生执行。</span><span class="sxs-lookup"><span data-stu-id="75002-106">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="75002-107">如果未将 **allowStudentsToAddResources** 标志设置为 ，此操作将不会成功 `true` 。</span><span class="sxs-lookup"><span data-stu-id="75002-107">This action will not succeed if the **allowStudentsToAddResources** flag isn't set to `true`.</span></span> <span data-ttu-id="75002-108">如果调用方想要创建新的基于文件的资源，则必须将该文件上载到与提交关联的资源文件夹。</span><span class="sxs-lookup"><span data-stu-id="75002-108">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="75002-109">如果文件不存在或不在该文件夹中，POST 请求将失败。</span><span class="sxs-lookup"><span data-stu-id="75002-109">If the file does not exist or isn't in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="75002-110">权限</span><span class="sxs-lookup"><span data-stu-id="75002-110">Permissions</span></span>
<span data-ttu-id="75002-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75002-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75002-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="75002-113">Permission type</span></span>      | <span data-ttu-id="75002-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75002-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75002-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75002-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="75002-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75002-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="75002-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75002-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75002-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="75002-118">Not supported.</span></span>  |
|<span data-ttu-id="75002-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="75002-119">Application</span></span> | <span data-ttu-id="75002-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="75002-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="75002-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75002-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="request-headers"></a><span data-ttu-id="75002-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="75002-122">Request headers</span></span>
| <span data-ttu-id="75002-123">标头</span><span class="sxs-lookup"><span data-stu-id="75002-123">Header</span></span>       | <span data-ttu-id="75002-124">值</span><span class="sxs-lookup"><span data-stu-id="75002-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75002-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75002-125">Authorization</span></span>  | <span data-ttu-id="75002-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75002-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="75002-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75002-128">Content-Type</span></span>  | <span data-ttu-id="75002-129">application/json</span><span class="sxs-lookup"><span data-stu-id="75002-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75002-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="75002-130">Request body</span></span>
<span data-ttu-id="75002-131">在请求正文中，提供 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75002-131">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="75002-132">响应</span><span class="sxs-lookup"><span data-stu-id="75002-132">Response</span></span>
<span data-ttu-id="75002-133">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75002-133">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75002-134">示例</span><span class="sxs-lookup"><span data-stu-id="75002-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="75002-135">请求</span><span class="sxs-lookup"><span data-stu-id="75002-135">Request</span></span>
<span data-ttu-id="75002-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="75002-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75002-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="75002-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  },
  "@odata.type": "microsoft.graph.educationResource"
}
```
# <a name="c"></a>[<span data-ttu-id="75002-138">C#</span><span class="sxs-lookup"><span data-stu-id="75002-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationsubmissionresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75002-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75002-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationsubmissionresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75002-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75002-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationsubmissionresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75002-141">Java</span><span class="sxs-lookup"><span data-stu-id="75002-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationsubmissionresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75002-142">响应</span><span class="sxs-lookup"><span data-stu-id="75002-142">Response</span></span>
<span data-ttu-id="75002-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="75002-143">The following is an example of the response.</span></span> 

><span data-ttu-id="75002-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="75002-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


