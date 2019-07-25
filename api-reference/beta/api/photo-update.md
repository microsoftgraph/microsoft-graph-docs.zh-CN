---
title: 更新照片
description: 更新 photo 对象的属性。
localization_priority: Normal
ms.openlocfilehash: 0d12b83f7c9436cce14a27ed5f27741b4ac92da3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876902"
---
# <a name="update-photo"></a><span data-ttu-id="a3f12-103">更新照片</span><span class="sxs-lookup"><span data-stu-id="a3f12-103">Update photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3f12-104">更新 photo 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a3f12-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3f12-105">权限</span><span class="sxs-lookup"><span data-stu-id="a3f12-105">Permissions</span></span>
<span data-ttu-id="a3f12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3f12-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3f12-108">Permission type</span></span>      | <span data-ttu-id="a3f12-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3f12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3f12-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3f12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3f12-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3f12-111">Not supported.</span></span>    |
|<span data-ttu-id="a3f12-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3f12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3f12-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3f12-113">Not supported.</span></span>    |
|<span data-ttu-id="a3f12-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3f12-114">Application</span></span> | <span data-ttu-id="a3f12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3f12-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3f12-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3f12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="a3f12-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3f12-117">Request headers</span></span>
| <span data-ttu-id="a3f12-118">名称</span><span class="sxs-lookup"><span data-stu-id="a3f12-118">Name</span></span>       | <span data-ttu-id="a3f12-119">类型</span><span class="sxs-lookup"><span data-stu-id="a3f12-119">Type</span></span> | <span data-ttu-id="a3f12-120">说明</span><span class="sxs-lookup"><span data-stu-id="a3f12-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a3f12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3f12-121">Authorization</span></span>  | <span data-ttu-id="a3f12-122">string</span><span class="sxs-lookup"><span data-stu-id="a3f12-122">string</span></span>  | <span data-ttu-id="a3f12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3f12-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3f12-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3f12-125">Request body</span></span>
<span data-ttu-id="a3f12-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a3f12-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a3f12-129">属性</span><span class="sxs-lookup"><span data-stu-id="a3f12-129">Property</span></span>     | <span data-ttu-id="a3f12-130">类型</span><span class="sxs-lookup"><span data-stu-id="a3f12-130">Type</span></span>   |<span data-ttu-id="a3f12-131">说明</span><span class="sxs-lookup"><span data-stu-id="a3f12-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="a3f12-132">响应</span><span class="sxs-lookup"><span data-stu-id="a3f12-132">Response</span></span>

<span data-ttu-id="a3f12-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3f12-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3f12-134">示例</span><span class="sxs-lookup"><span data-stu-id="a3f12-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3f12-135">请求</span><span class="sxs-lookup"><span data-stu-id="a3f12-135">Request</span></span>
<span data-ttu-id="a3f12-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3f12-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a3f12-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a3f12-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3f12-138">C#</span><span class="sxs-lookup"><span data-stu-id="a3f12-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3f12-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3f12-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3f12-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="a3f12-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3f12-141">Java</span><span class="sxs-lookup"><span data-stu-id="a3f12-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a3f12-142">响应</span><span class="sxs-lookup"><span data-stu-id="a3f12-142">Response</span></span>
<span data-ttu-id="a3f12-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a3f12-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
