---
title: 更新 educationAssignmentResource
description: '更新与工作分配关联的资源的属性。 只有班级中的教师可以更改作业资源对象。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5dae821a6dc22aa108bceee44c4958e3deb7f129
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52733000"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="8e0b6-104">更新 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="8e0b6-104">Update educationAssignmentResource</span></span>

<span data-ttu-id="8e0b6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e0b6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e0b6-106">更新与工作分配关联的资源的属性。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-106">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="8e0b6-107">只有班级中的教师可以更改作业资源对象。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-107">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="8e0b6-108">权限</span><span class="sxs-lookup"><span data-stu-id="8e0b6-108">Permissions</span></span>
<span data-ttu-id="8e0b6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e0b6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e0b6-111">Permission type</span></span>      | <span data-ttu-id="8e0b6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e0b6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e0b6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e0b6-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8e0b6-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e0b6-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8e0b6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e0b6-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8e0b6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-116">Not supported.</span></span>  |
|<span data-ttu-id="8e0b6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e0b6-117">Application</span></span> | <span data-ttu-id="8e0b6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8e0b6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e0b6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8e0b6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e0b6-120">Request headers</span></span>
| <span data-ttu-id="8e0b6-121">标头</span><span class="sxs-lookup"><span data-stu-id="8e0b6-121">Header</span></span>       | <span data-ttu-id="8e0b6-122">值</span><span class="sxs-lookup"><span data-stu-id="8e0b6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e0b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e0b6-123">Authorization</span></span>  | <span data-ttu-id="8e0b6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8e0b6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e0b6-126">Content-Type</span></span>  | <span data-ttu-id="8e0b6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8e0b6-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e0b6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e0b6-128">Request body</span></span>
<span data-ttu-id="8e0b6-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8e0b6-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8e0b6-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e0b6-132">属性</span><span class="sxs-lookup"><span data-stu-id="8e0b6-132">Property</span></span>     | <span data-ttu-id="8e0b6-133">类型</span><span class="sxs-lookup"><span data-stu-id="8e0b6-133">Type</span></span>   |<span data-ttu-id="8e0b6-134">说明</span><span class="sxs-lookup"><span data-stu-id="8e0b6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e0b6-135">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="8e0b6-135">distributeForStudentWork</span></span>|<span data-ttu-id="8e0b6-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e0b6-136">Boolean</span></span>| <span data-ttu-id="8e0b6-137">指示发布作业时，是否应该将此资源复制到每个学生的资源对象。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-137">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="8e0b6-138">resource</span><span class="sxs-lookup"><span data-stu-id="8e0b6-138">resource</span></span>|<span data-ttu-id="8e0b6-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="8e0b6-139">educationResource</span></span>| <span data-ttu-id="8e0b6-140">Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-140">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="8e0b6-141">响应</span><span class="sxs-lookup"><span data-stu-id="8e0b6-141">Response</span></span>
<span data-ttu-id="8e0b6-142">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-142">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e0b6-143">示例</span><span class="sxs-lookup"><span data-stu-id="8e0b6-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e0b6-144">请求</span><span class="sxs-lookup"><span data-stu-id="8e0b6-144">Request</span></span>
<span data-ttu-id="8e0b6-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e0b6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e0b6-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentresource"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf
Content-type: application/json
Content-length: 822

{
  "distributeForStudentWork": "false"
}
```
# <a name="c"></a>[<span data-ttu-id="8e0b6-147">C#</span><span class="sxs-lookup"><span data-stu-id="8e0b6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e0b6-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e0b6-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e0b6-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e0b6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e0b6-150">Java</span><span class="sxs-lookup"><span data-stu-id="8e0b6-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e0b6-151">响应</span><span class="sxs-lookup"><span data-stu-id="8e0b6-151">Response</span></span>
<span data-ttu-id="8e0b6-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-152">The following is an example of the response.</span></span> 

><span data-ttu-id="8e0b6-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e0b6-153">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 832

{
  "distributeForStudentWork": false,
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
  "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


