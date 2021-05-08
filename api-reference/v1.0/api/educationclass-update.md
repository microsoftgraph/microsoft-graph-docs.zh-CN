---
title: 更新 educationClass
description: 更新课程属性。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5340a05df5068942c2f895c9858e2f5cd280e24a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231960"
---
# <a name="update-educationclass"></a><span data-ttu-id="e76b2-103">更新 educationClass</span><span class="sxs-lookup"><span data-stu-id="e76b2-103">Update educationClass</span></span>

<span data-ttu-id="e76b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e76b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e76b2-105">更新 [educationClass 对象](../resources/educationclass.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e76b2-105">Update the properties of an [educationClass](../resources/educationclass.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e76b2-106">权限</span><span class="sxs-lookup"><span data-stu-id="e76b2-106">Permissions</span></span>
<span data-ttu-id="e76b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e76b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76b2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e76b2-109">Permission type</span></span>      | <span data-ttu-id="e76b2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e76b2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e76b2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e76b2-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e76b2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e76b2-112">Not supported.</span></span>  |
|<span data-ttu-id="e76b2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e76b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e76b2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e76b2-114">Not supported.</span></span>   |
|<span data-ttu-id="e76b2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e76b2-115">Application</span></span> | <span data-ttu-id="e76b2-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76b2-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e76b2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e76b2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e76b2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e76b2-118">Request headers</span></span>
| <span data-ttu-id="e76b2-119">标头</span><span class="sxs-lookup"><span data-stu-id="e76b2-119">Header</span></span>       | <span data-ttu-id="e76b2-120">值</span><span class="sxs-lookup"><span data-stu-id="e76b2-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e76b2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e76b2-121">Authorization</span></span>  | <span data-ttu-id="e76b2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e76b2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e76b2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e76b2-124">Content-Type</span></span>  | <span data-ttu-id="e76b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e76b2-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e76b2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e76b2-126">Request body</span></span>
<span data-ttu-id="e76b2-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e76b2-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e76b2-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e76b2-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e76b2-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e76b2-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e76b2-130">属性</span><span class="sxs-lookup"><span data-stu-id="e76b2-130">Property</span></span>             | <span data-ttu-id="e76b2-131">类型</span><span class="sxs-lookup"><span data-stu-id="e76b2-131">Type</span></span>                                               | <span data-ttu-id="e76b2-132">说明</span><span class="sxs-lookup"><span data-stu-id="e76b2-132">Description</span></span>                                                        |
| :------------------- | :------------------------------------------------- | :----------------------------------------------------------------- |
| <span data-ttu-id="e76b2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e76b2-133">displayName</span></span>          | <span data-ttu-id="e76b2-134">String</span><span class="sxs-lookup"><span data-stu-id="e76b2-134">String</span></span>                                             | <span data-ttu-id="e76b2-135">课程名称。</span><span class="sxs-lookup"><span data-stu-id="e76b2-135">Name of the class.</span></span>                                                 |
| <span data-ttu-id="e76b2-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e76b2-136">mailNickname</span></span>         | <span data-ttu-id="e76b2-137">String</span><span class="sxs-lookup"><span data-stu-id="e76b2-137">String</span></span>                                             | <span data-ttu-id="e76b2-138">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="e76b2-138">Mail name for sending email to all members, if this is enabled.</span></span>    |
| <span data-ttu-id="e76b2-139">说明</span><span class="sxs-lookup"><span data-stu-id="e76b2-139">description</span></span>          | <span data-ttu-id="e76b2-140">String</span><span class="sxs-lookup"><span data-stu-id="e76b2-140">String</span></span>                                             | <span data-ttu-id="e76b2-141">课程说明。</span><span class="sxs-lookup"><span data-stu-id="e76b2-141">Description of the class.</span></span>                                          |
| <span data-ttu-id="e76b2-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="e76b2-142">createdBy</span></span>            | [<span data-ttu-id="e76b2-143">identitySet</span><span class="sxs-lookup"><span data-stu-id="e76b2-143">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="e76b2-144">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="e76b2-144">Entity who created the class</span></span>                                       |
| <span data-ttu-id="e76b2-145">classCode</span><span class="sxs-lookup"><span data-stu-id="e76b2-145">classCode</span></span>            | <span data-ttu-id="e76b2-146">String</span><span class="sxs-lookup"><span data-stu-id="e76b2-146">String</span></span>                                             | <span data-ttu-id="e76b2-147">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="e76b2-147">Class code used by the school to identify the class.</span></span>               |
| <span data-ttu-id="e76b2-148">externalId</span><span class="sxs-lookup"><span data-stu-id="e76b2-148">externalId</span></span>           | <span data-ttu-id="e76b2-149">String</span><span class="sxs-lookup"><span data-stu-id="e76b2-149">String</span></span>                                             | <span data-ttu-id="e76b2-150">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="e76b2-150">ID of the class from the syncing system.</span></span>                           |
| <span data-ttu-id="e76b2-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="e76b2-151">externalSource</span></span>       | <span data-ttu-id="e76b2-152">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="e76b2-152">educationExternalSource</span></span>                            | <span data-ttu-id="e76b2-153">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="e76b2-153">How this class was created.</span></span> <span data-ttu-id="e76b2-154">可能的值包括： `sis` 、 `manual`</span><span class="sxs-lookup"><span data-stu-id="e76b2-154">Possible values are: `sis`, `manual`</span></span>   |
| <span data-ttu-id="e76b2-155">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="e76b2-155">externalSourceDetail</span></span> | <span data-ttu-id="e76b2-156">String</span><span class="sxs-lookup"><span data-stu-id="e76b2-156">String</span></span>                                             | <span data-ttu-id="e76b2-157">生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="e76b2-157">The name of the external source this resources was generated from.</span></span> |
| <span data-ttu-id="e76b2-158">grade</span><span class="sxs-lookup"><span data-stu-id="e76b2-158">grade</span></span>                | <span data-ttu-id="e76b2-159">String</span><span class="sxs-lookup"><span data-stu-id="e76b2-159">String</span></span>                                             | <span data-ttu-id="e76b2-160">课程的年级。</span><span class="sxs-lookup"><span data-stu-id="e76b2-160">Grade level of the class.</span></span>                                          |
| <span data-ttu-id="e76b2-161">term</span><span class="sxs-lookup"><span data-stu-id="e76b2-161">term</span></span>                 | [<span data-ttu-id="e76b2-162">educationTerm</span><span class="sxs-lookup"><span data-stu-id="e76b2-162">educationTerm</span></span>](../resources/educationterm.md)     | <span data-ttu-id="e76b2-163">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="e76b2-163">Term for this class.</span></span>                                               |

## <a name="response"></a><span data-ttu-id="e76b2-164">响应</span><span class="sxs-lookup"><span data-stu-id="e76b2-164">Response</span></span>
<span data-ttu-id="e76b2-165">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e76b2-165">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e76b2-166">示例</span><span class="sxs-lookup"><span data-stu-id="e76b2-166">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e76b2-167">请求</span><span class="sxs-lookup"><span data-stu-id="e76b2-167">Request</span></span>
<span data-ttu-id="e76b2-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e76b2-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e76b2-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="e76b2-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
# <a name="c"></a>[<span data-ttu-id="e76b2-170">C#</span><span class="sxs-lookup"><span data-stu-id="e76b2-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e76b2-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e76b2-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e76b2-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e76b2-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e76b2-173">Java</span><span class="sxs-lookup"><span data-stu-id="e76b2-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e76b2-174">响应</span><span class="sxs-lookup"><span data-stu-id="e76b2-174">Response</span></span>
<span data-ttu-id="e76b2-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e76b2-175">The following is an example of the response.</span></span> 

><span data-ttu-id="e76b2-176">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e76b2-176">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
