---
title: 更新 educationclass 属性
description: 更新课程属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 452c534e765f1947a3cd224abc024865e5a887df
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441616"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="6794e-103">更新 educationclass 属性</span><span class="sxs-lookup"><span data-stu-id="6794e-103">Update educationclass properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6794e-104">更新课程属性。</span><span class="sxs-lookup"><span data-stu-id="6794e-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="6794e-105">权限</span><span class="sxs-lookup"><span data-stu-id="6794e-105">Permissions</span></span>
<span data-ttu-id="6794e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6794e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6794e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6794e-108">Permission type</span></span>      | <span data-ttu-id="6794e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6794e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6794e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6794e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6794e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="6794e-111">Not supported.</span></span>  |
|<span data-ttu-id="6794e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6794e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6794e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6794e-113">Not supported.</span></span>   |
|<span data-ttu-id="6794e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6794e-114">Application</span></span> | <span data-ttu-id="6794e-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6794e-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6794e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6794e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6794e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6794e-117">Request headers</span></span>
| <span data-ttu-id="6794e-118">标头</span><span class="sxs-lookup"><span data-stu-id="6794e-118">Header</span></span>       | <span data-ttu-id="6794e-119">值</span><span class="sxs-lookup"><span data-stu-id="6794e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6794e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6794e-120">Authorization</span></span>  | <span data-ttu-id="6794e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6794e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6794e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6794e-123">Content-Type</span></span>  | <span data-ttu-id="6794e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6794e-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6794e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6794e-125">Request body</span></span>
<span data-ttu-id="6794e-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="6794e-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6794e-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="6794e-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6794e-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6794e-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6794e-129">属性</span><span class="sxs-lookup"><span data-stu-id="6794e-129">Property</span></span>     | <span data-ttu-id="6794e-130">类型</span><span class="sxs-lookup"><span data-stu-id="6794e-130">Type</span></span>   |<span data-ttu-id="6794e-131">说明</span><span class="sxs-lookup"><span data-stu-id="6794e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6794e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6794e-132">description</span></span>|<span data-ttu-id="6794e-133">String</span><span class="sxs-lookup"><span data-stu-id="6794e-133">String</span></span>| <span data-ttu-id="6794e-134">课程说明。</span><span class="sxs-lookup"><span data-stu-id="6794e-134">Description of the class.</span></span>|
|<span data-ttu-id="6794e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6794e-135">displayName</span></span>|<span data-ttu-id="6794e-136">String</span><span class="sxs-lookup"><span data-stu-id="6794e-136">String</span></span>| <span data-ttu-id="6794e-137">课程名称。</span><span class="sxs-lookup"><span data-stu-id="6794e-137">Name of the class.</span></span>|
|<span data-ttu-id="6794e-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6794e-138">mailNickname</span></span>|<span data-ttu-id="6794e-139">String</span><span class="sxs-lookup"><span data-stu-id="6794e-139">String</span></span>| <span data-ttu-id="6794e-140">用于向所有用户发送电子邮件的电子邮件别名（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="6794e-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="6794e-141">|classCode|String| 由学校使用的课程代码。| |externalId|String| 来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="6794e-141">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="6794e-142">| |externalName|String|同步系统中的课程名称。| |externalSource|string| 此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="6794e-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="6794e-143">可取值为：`sis`、`manual`、`enum_sentinel`。|</span><span class="sxs-lookup"><span data-stu-id="6794e-143">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="6794e-144">响应</span><span class="sxs-lookup"><span data-stu-id="6794e-144">Response</span></span>
<span data-ttu-id="6794e-145">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6794e-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6794e-146">示例</span><span class="sxs-lookup"><span data-stu-id="6794e-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6794e-147">请求</span><span class="sxs-lookup"><span data-stu-id="6794e-147">Request</span></span>
<span data-ttu-id="6794e-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6794e-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6794e-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6794e-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6794e-150">C#</span><span class="sxs-lookup"><span data-stu-id="6794e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6794e-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="6794e-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6794e-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="6794e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6794e-153">响应</span><span class="sxs-lookup"><span data-stu-id="6794e-153">Response</span></span>
<span data-ttu-id="6794e-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6794e-154">The following is an example of the response.</span></span> 

><span data-ttu-id="6794e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6794e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
