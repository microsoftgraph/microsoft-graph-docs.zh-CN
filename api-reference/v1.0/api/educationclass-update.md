---
title: 更新 educationclass 属性
description: 更新课程属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2e0e6dff51e16f0582e2bbbde058f8e78f35d5c1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051457"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="d6eaa-103">更新 educationclass 属性</span><span class="sxs-lookup"><span data-stu-id="d6eaa-103">Update educationclass properties</span></span>

<span data-ttu-id="d6eaa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6eaa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6eaa-105">更新课程属性。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-105">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6eaa-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6eaa-106">Permissions</span></span>
<span data-ttu-id="d6eaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6eaa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6eaa-109">Permission type</span></span>      | <span data-ttu-id="d6eaa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6eaa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6eaa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6eaa-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d6eaa-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-112">Not supported.</span></span>  |
|<span data-ttu-id="d6eaa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6eaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6eaa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-114">Not supported.</span></span>   |
|<span data-ttu-id="d6eaa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6eaa-115">Application</span></span> | <span data-ttu-id="d6eaa-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6eaa-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d6eaa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6eaa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d6eaa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6eaa-118">Request headers</span></span>
| <span data-ttu-id="d6eaa-119">标头</span><span class="sxs-lookup"><span data-stu-id="d6eaa-119">Header</span></span>       | <span data-ttu-id="d6eaa-120">值</span><span class="sxs-lookup"><span data-stu-id="d6eaa-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d6eaa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6eaa-121">Authorization</span></span>  | <span data-ttu-id="d6eaa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6eaa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6eaa-124">Content-Type</span></span>  | <span data-ttu-id="d6eaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6eaa-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6eaa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6eaa-126">Request body</span></span>
<span data-ttu-id="d6eaa-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d6eaa-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d6eaa-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d6eaa-130">属性</span><span class="sxs-lookup"><span data-stu-id="d6eaa-130">Property</span></span>     | <span data-ttu-id="d6eaa-131">类型</span><span class="sxs-lookup"><span data-stu-id="d6eaa-131">Type</span></span>   |<span data-ttu-id="d6eaa-132">说明</span><span class="sxs-lookup"><span data-stu-id="d6eaa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6eaa-133">说明</span><span class="sxs-lookup"><span data-stu-id="d6eaa-133">description</span></span>|<span data-ttu-id="d6eaa-134">String</span><span class="sxs-lookup"><span data-stu-id="d6eaa-134">String</span></span>| <span data-ttu-id="d6eaa-135">课程说明。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-135">Description of the class.</span></span>|
|<span data-ttu-id="d6eaa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d6eaa-136">displayName</span></span>|<span data-ttu-id="d6eaa-137">String</span><span class="sxs-lookup"><span data-stu-id="d6eaa-137">String</span></span>| <span data-ttu-id="d6eaa-138">课程名称。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-138">Name of the class.</span></span>|
|<span data-ttu-id="d6eaa-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d6eaa-139">mailNickname</span></span>|<span data-ttu-id="d6eaa-140">String</span><span class="sxs-lookup"><span data-stu-id="d6eaa-140">String</span></span>| <span data-ttu-id="d6eaa-141">用于向所有用户发送电子邮件的电子邮件别名（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-141">Email alias for sending email to all users if that feature is enabled.</span></span> |
|<span data-ttu-id="d6eaa-142">classCode</span><span class="sxs-lookup"><span data-stu-id="d6eaa-142">classCode</span></span>|<span data-ttu-id="d6eaa-143">String</span><span class="sxs-lookup"><span data-stu-id="d6eaa-143">String</span></span>| <span data-ttu-id="d6eaa-144">学校使用的课堂代码。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-144">Class code used by the school.</span></span>|
|<span data-ttu-id="d6eaa-145">externalId</span><span class="sxs-lookup"><span data-stu-id="d6eaa-145">externalId</span></span>|<span data-ttu-id="d6eaa-146">String</span><span class="sxs-lookup"><span data-stu-id="d6eaa-146">String</span></span>| <span data-ttu-id="d6eaa-147">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-147">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="d6eaa-148">externalName</span><span class="sxs-lookup"><span data-stu-id="d6eaa-148">externalName</span></span>|<span data-ttu-id="d6eaa-149">String</span><span class="sxs-lookup"><span data-stu-id="d6eaa-149">String</span></span>|<span data-ttu-id="d6eaa-150">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-150">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="d6eaa-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="d6eaa-151">externalSource</span></span>|<span data-ttu-id="d6eaa-152">string</span><span class="sxs-lookup"><span data-stu-id="d6eaa-152">string</span></span>| <span data-ttu-id="d6eaa-153">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-153">How this class was created.</span></span> <span data-ttu-id="d6eaa-154">可能的值包括 `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-154">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|

## <a name="response"></a><span data-ttu-id="d6eaa-155">响应</span><span class="sxs-lookup"><span data-stu-id="d6eaa-155">Response</span></span>
<span data-ttu-id="d6eaa-156">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-156">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6eaa-157">示例</span><span class="sxs-lookup"><span data-stu-id="d6eaa-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6eaa-158">请求</span><span class="sxs-lookup"><span data-stu-id="d6eaa-158">Request</span></span>
<span data-ttu-id="d6eaa-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6eaa-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6eaa-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d6eaa-161">C#</span><span class="sxs-lookup"><span data-stu-id="d6eaa-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6eaa-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6eaa-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6eaa-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6eaa-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6eaa-164">Java</span><span class="sxs-lookup"><span data-stu-id="d6eaa-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6eaa-165">响应</span><span class="sxs-lookup"><span data-stu-id="d6eaa-165">Response</span></span>
<span data-ttu-id="d6eaa-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-166">The following is an example of the response.</span></span> 

><span data-ttu-id="d6eaa-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d6eaa-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
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

