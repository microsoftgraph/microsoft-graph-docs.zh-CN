---
title: 获取 educationSubmissionResource
description: 检索与提交关联的特定资源的属性。 此资源位于"工作"资源列表中，应视为学生正在处理的工作。 如果此资源是从工作分配复制的，则用可能的指针将资源打包回工作分配资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 31df23948009f8724b1bf08a8608fc9ae0b316be
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061859"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="6b7a4-105">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="6b7a4-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="6b7a4-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b7a4-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b7a4-107">检索与提交关联的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="6b7a4-108">此资源位于"工作"资源列表中，应视为学生正在处理的工作。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="6b7a4-109">如果此资源是从工作分配复制的，则用可能的指针将资源打包回工作分配资源。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b7a4-110">权限</span><span class="sxs-lookup"><span data-stu-id="6b7a4-110">Permissions</span></span>
<span data-ttu-id="6b7a4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b7a4-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b7a4-113">Permission type</span></span>      | <span data-ttu-id="6b7a4-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b7a4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b7a4-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b7a4-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="6b7a4-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b7a4-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6b7a4-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b7a4-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6b7a4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-118">Not supported.</span></span>  |
|<span data-ttu-id="6b7a4-119">Application\*</span><span class="sxs-lookup"><span data-stu-id="6b7a4-119">Application\*</span></span> | <span data-ttu-id="6b7a4-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b7a4-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="6b7a4-121">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b7a4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b7a4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b7a4-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6b7a4-123">Optional query parameters</span></span>
<span data-ttu-id="6b7a4-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b7a4-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b7a4-125">Request headers</span></span>
| <span data-ttu-id="6b7a4-126">标头</span><span class="sxs-lookup"><span data-stu-id="6b7a4-126">Header</span></span>       | <span data-ttu-id="6b7a4-127">值</span><span class="sxs-lookup"><span data-stu-id="6b7a4-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b7a4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b7a4-128">Authorization</span></span>  | <span data-ttu-id="6b7a4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b7a4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b7a4-131">Request body</span></span>
<span data-ttu-id="6b7a4-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6b7a4-133">响应</span><span class="sxs-lookup"><span data-stu-id="6b7a4-133">Response</span></span>
<span data-ttu-id="6b7a4-134">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b7a4-135">示例</span><span class="sxs-lookup"><span data-stu-id="6b7a4-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b7a4-136">请求</span><span class="sxs-lookup"><span data-stu-id="6b7a4-136">Request</span></span>
<span data-ttu-id="6b7a4-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b7a4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b7a4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="6b7a4-139">C#</span><span class="sxs-lookup"><span data-stu-id="6b7a4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b7a4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b7a4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b7a4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b7a4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b7a4-142">Java</span><span class="sxs-lookup"><span data-stu-id="6b7a4-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b7a4-143">响应</span><span class="sxs-lookup"><span data-stu-id="6b7a4-143">Response</span></span>
<span data-ttu-id="6b7a4-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-144">The following is an example of the response.</span></span> 

><span data-ttu-id="6b7a4-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b7a4-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
