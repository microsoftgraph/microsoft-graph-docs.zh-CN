---
title: 更新 educationclass 属性
description: 更新课程属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e8b5e6508af5b00ecdcd50180d8a5ed47c05c009
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810893"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="ae409-103">更新 educationclass 属性</span><span class="sxs-lookup"><span data-stu-id="ae409-103">Update educationclass properties</span></span>

<span data-ttu-id="ae409-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae409-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae409-105">更新课程属性。</span><span class="sxs-lookup"><span data-stu-id="ae409-105">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae409-106">权限</span><span class="sxs-lookup"><span data-stu-id="ae409-106">Permissions</span></span>
<span data-ttu-id="ae409-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae409-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae409-109">Permission type</span></span>      | <span data-ttu-id="ae409-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae409-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae409-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae409-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ae409-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae409-112">Not supported.</span></span>  |
|<span data-ttu-id="ae409-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae409-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae409-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae409-114">Not supported.</span></span>   |
|<span data-ttu-id="ae409-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae409-115">Application</span></span> | <span data-ttu-id="ae409-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae409-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae409-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae409-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ae409-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae409-118">Request headers</span></span>
| <span data-ttu-id="ae409-119">标头</span><span class="sxs-lookup"><span data-stu-id="ae409-119">Header</span></span>       | <span data-ttu-id="ae409-120">值</span><span class="sxs-lookup"><span data-stu-id="ae409-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae409-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae409-121">Authorization</span></span>  | <span data-ttu-id="ae409-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae409-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae409-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae409-124">Content-Type</span></span>  | <span data-ttu-id="ae409-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae409-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae409-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae409-126">Request body</span></span>
<span data-ttu-id="ae409-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ae409-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ae409-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ae409-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ae409-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ae409-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ae409-130">属性</span><span class="sxs-lookup"><span data-stu-id="ae409-130">Property</span></span>     | <span data-ttu-id="ae409-131">类型</span><span class="sxs-lookup"><span data-stu-id="ae409-131">Type</span></span>   |<span data-ttu-id="ae409-132">说明</span><span class="sxs-lookup"><span data-stu-id="ae409-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae409-133">说明</span><span class="sxs-lookup"><span data-stu-id="ae409-133">description</span></span>|<span data-ttu-id="ae409-134">String</span><span class="sxs-lookup"><span data-stu-id="ae409-134">String</span></span>| <span data-ttu-id="ae409-135">课程说明。</span><span class="sxs-lookup"><span data-stu-id="ae409-135">Description of the class.</span></span>|
|<span data-ttu-id="ae409-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ae409-136">displayName</span></span>|<span data-ttu-id="ae409-137">String</span><span class="sxs-lookup"><span data-stu-id="ae409-137">String</span></span>| <span data-ttu-id="ae409-138">课程名称。</span><span class="sxs-lookup"><span data-stu-id="ae409-138">Name of the class.</span></span>|
|<span data-ttu-id="ae409-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ae409-139">mailNickname</span></span>|<span data-ttu-id="ae409-140">String</span><span class="sxs-lookup"><span data-stu-id="ae409-140">String</span></span>| <span data-ttu-id="ae409-141">用于向所有用户发送电子邮件的电子邮件别名（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="ae409-141">Email alias for sending email to all users if that feature is enabled.</span></span> |
|<span data-ttu-id="ae409-142">classCode</span><span class="sxs-lookup"><span data-stu-id="ae409-142">classCode</span></span>|<span data-ttu-id="ae409-143">String</span><span class="sxs-lookup"><span data-stu-id="ae409-143">String</span></span>| <span data-ttu-id="ae409-144">学校使用的类代码。</span><span class="sxs-lookup"><span data-stu-id="ae409-144">Class code used by the school.</span></span>|
|<span data-ttu-id="ae409-145">externalId</span><span class="sxs-lookup"><span data-stu-id="ae409-145">externalId</span></span>|<span data-ttu-id="ae409-146">String</span><span class="sxs-lookup"><span data-stu-id="ae409-146">String</span></span>| <span data-ttu-id="ae409-147">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="ae409-147">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="ae409-148">externalName</span><span class="sxs-lookup"><span data-stu-id="ae409-148">externalName</span></span>|<span data-ttu-id="ae409-149">String</span><span class="sxs-lookup"><span data-stu-id="ae409-149">String</span></span>|<span data-ttu-id="ae409-150">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="ae409-150">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="ae409-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="ae409-151">externalSource</span></span>|<span data-ttu-id="ae409-152">string</span><span class="sxs-lookup"><span data-stu-id="ae409-152">string</span></span>| <span data-ttu-id="ae409-153">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="ae409-153">How this class was created.</span></span> <span data-ttu-id="ae409-154">可取值为：`sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="ae409-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|

## <a name="response"></a><span data-ttu-id="ae409-155">响应</span><span class="sxs-lookup"><span data-stu-id="ae409-155">Response</span></span>
<span data-ttu-id="ae409-156">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae409-156">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae409-157">示例</span><span class="sxs-lookup"><span data-stu-id="ae409-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae409-158">请求</span><span class="sxs-lookup"><span data-stu-id="ae409-158">Request</span></span>
<span data-ttu-id="ae409-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae409-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae409-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae409-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
# <a name="c"></a>[<span data-ttu-id="ae409-161">C#</span><span class="sxs-lookup"><span data-stu-id="ae409-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae409-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae409-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae409-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae409-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ae409-164">响应</span><span class="sxs-lookup"><span data-stu-id="ae409-164">Response</span></span>
<span data-ttu-id="ae409-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ae409-165">The following is an example of the response.</span></span>

><span data-ttu-id="ae409-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae409-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
          "id": "14012",
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
<!--
{
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
