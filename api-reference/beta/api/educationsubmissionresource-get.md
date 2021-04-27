---
title: 获取 educationSubmissionResource
description: 检索与提交关联的特定资源的属性。 此资源位于"工作"资源列表中，应视为学生正在处理的工作。 如果此资源是从工作分配复制的，则用可能的指针将资源打包回工作分配资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 29108fbcef7bc3a36ca2021a0e019abd4206c12a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043183"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="d38f4-105">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d38f4-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="d38f4-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d38f4-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38f4-107">检索与提交关联的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d38f4-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="d38f4-108">此资源位于"工作"资源列表中，应视为学生正在处理的工作。</span><span class="sxs-lookup"><span data-stu-id="d38f4-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="d38f4-109">如果此资源是从工作分配复制的，则用可能的指针将资源打包回工作分配资源。</span><span class="sxs-lookup"><span data-stu-id="d38f4-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d38f4-110">权限</span><span class="sxs-lookup"><span data-stu-id="d38f4-110">Permissions</span></span>
<span data-ttu-id="d38f4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d38f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38f4-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d38f4-113">Permission type</span></span>      | <span data-ttu-id="d38f4-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d38f4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d38f4-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d38f4-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d38f4-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d38f4-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d38f4-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d38f4-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d38f4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d38f4-118">Not supported.</span></span>  |
|<span data-ttu-id="d38f4-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d38f4-119">Application</span></span> | <span data-ttu-id="d38f4-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d38f4-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d38f4-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d38f4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d38f4-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d38f4-122">Optional query parameters</span></span>
<span data-ttu-id="d38f4-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d38f4-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d38f4-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d38f4-124">Request headers</span></span>
| <span data-ttu-id="d38f4-125">标头</span><span class="sxs-lookup"><span data-stu-id="d38f4-125">Header</span></span>       | <span data-ttu-id="d38f4-126">值</span><span class="sxs-lookup"><span data-stu-id="d38f4-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d38f4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d38f4-127">Authorization</span></span>  | <span data-ttu-id="d38f4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d38f4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d38f4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d38f4-130">Request body</span></span>
<span data-ttu-id="d38f4-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d38f4-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d38f4-132">响应</span><span class="sxs-lookup"><span data-stu-id="d38f4-132">Response</span></span>
<span data-ttu-id="d38f4-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d38f4-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d38f4-134">示例</span><span class="sxs-lookup"><span data-stu-id="d38f4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d38f4-135">请求</span><span class="sxs-lookup"><span data-stu-id="d38f4-135">Request</span></span>
<span data-ttu-id="d38f4-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d38f4-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d38f4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d38f4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="d38f4-138">C#</span><span class="sxs-lookup"><span data-stu-id="d38f4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d38f4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d38f4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d38f4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d38f4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d38f4-141">Java</span><span class="sxs-lookup"><span data-stu-id="d38f4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d38f4-142">响应</span><span class="sxs-lookup"><span data-stu-id="d38f4-142">Response</span></span>
<span data-ttu-id="d38f4-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d38f4-143">The following is an example of the response.</span></span> 

><span data-ttu-id="d38f4-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d38f4-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
