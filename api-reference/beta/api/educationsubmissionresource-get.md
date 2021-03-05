---
title: 获取 educationSubmissionResource
description: 检索与提交关联的特定资源的属性。 此资源位于"工作"资源列表中，学生应认为正在工作。 如果此资源是从工作分配复制的，则使用可能指向工作分配资源的指针进行包装。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6f12b9b1739f844b5ef41e99942c3063f0cec95
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470360"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="6d503-105">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="6d503-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="6d503-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d503-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d503-107">检索与提交关联的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="6d503-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="6d503-108">此资源位于"工作"资源列表中，学生应认为正在工作。</span><span class="sxs-lookup"><span data-stu-id="6d503-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="6d503-109">如果此资源是从工作分配复制的，则使用可能指向工作分配资源的指针进行包装。</span><span class="sxs-lookup"><span data-stu-id="6d503-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d503-110">权限</span><span class="sxs-lookup"><span data-stu-id="6d503-110">Permissions</span></span>
<span data-ttu-id="6d503-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d503-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d503-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d503-113">Permission type</span></span>      | <span data-ttu-id="6d503-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d503-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d503-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d503-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="6d503-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d503-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6d503-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d503-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6d503-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d503-118">Not supported.</span></span>  |
|<span data-ttu-id="6d503-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d503-119">Application</span></span> | <span data-ttu-id="6d503-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d503-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6d503-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d503-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d503-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d503-122">Optional query parameters</span></span>
<span data-ttu-id="6d503-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6d503-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d503-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d503-124">Request headers</span></span>
| <span data-ttu-id="6d503-125">标头</span><span class="sxs-lookup"><span data-stu-id="6d503-125">Header</span></span>       | <span data-ttu-id="6d503-126">值</span><span class="sxs-lookup"><span data-stu-id="6d503-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d503-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d503-127">Authorization</span></span>  | <span data-ttu-id="6d503-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d503-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d503-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d503-130">Request body</span></span>
<span data-ttu-id="6d503-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d503-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6d503-132">响应</span><span class="sxs-lookup"><span data-stu-id="6d503-132">Response</span></span>
<span data-ttu-id="6d503-133">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d503-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d503-134">示例</span><span class="sxs-lookup"><span data-stu-id="6d503-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d503-135">请求</span><span class="sxs-lookup"><span data-stu-id="6d503-135">Request</span></span>
<span data-ttu-id="6d503-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6d503-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d503-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d503-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="6d503-138">C#</span><span class="sxs-lookup"><span data-stu-id="6d503-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d503-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d503-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d503-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d503-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d503-141">Java</span><span class="sxs-lookup"><span data-stu-id="6d503-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6d503-142">响应</span><span class="sxs-lookup"><span data-stu-id="6d503-142">Response</span></span>
<span data-ttu-id="6d503-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6d503-143">The following is an example of the response.</span></span> 

><span data-ttu-id="6d503-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6d503-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
