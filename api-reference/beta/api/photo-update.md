---
title: 更新照片
description: 更新 photo 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: MSGraphDocsVteam
ms.openlocfilehash: d13411227dde53a582af5f3614fe5a6f4a3051cd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811626"
---
# <a name="update-photo"></a><span data-ttu-id="1fac9-103">更新照片</span><span class="sxs-lookup"><span data-stu-id="1fac9-103">Update photo</span></span>

<span data-ttu-id="1fac9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fac9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fac9-105">更新 photo 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1fac9-105">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1fac9-106">权限</span><span class="sxs-lookup"><span data-stu-id="1fac9-106">Permissions</span></span>
<span data-ttu-id="1fac9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fac9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fac9-109">Permission type</span></span>      | <span data-ttu-id="1fac9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1fac9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fac9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fac9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1fac9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fac9-112">Not supported.</span></span>    |
|<span data-ttu-id="1fac9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fac9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fac9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fac9-114">Not supported.</span></span>    |
|<span data-ttu-id="1fac9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fac9-115">Application</span></span> | <span data-ttu-id="1fac9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fac9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fac9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fac9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="1fac9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fac9-118">Request headers</span></span>
| <span data-ttu-id="1fac9-119">名称</span><span class="sxs-lookup"><span data-stu-id="1fac9-119">Name</span></span>       | <span data-ttu-id="1fac9-120">类型</span><span class="sxs-lookup"><span data-stu-id="1fac9-120">Type</span></span> | <span data-ttu-id="1fac9-121">说明</span><span class="sxs-lookup"><span data-stu-id="1fac9-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1fac9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fac9-122">Authorization</span></span>  | <span data-ttu-id="1fac9-123">string</span><span class="sxs-lookup"><span data-stu-id="1fac9-123">string</span></span>  | <span data-ttu-id="1fac9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1fac9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fac9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fac9-126">Request body</span></span>
<span data-ttu-id="1fac9-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1fac9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1fac9-130">属性</span><span class="sxs-lookup"><span data-stu-id="1fac9-130">Property</span></span>     | <span data-ttu-id="1fac9-131">类型</span><span class="sxs-lookup"><span data-stu-id="1fac9-131">Type</span></span>   |<span data-ttu-id="1fac9-132">说明</span><span class="sxs-lookup"><span data-stu-id="1fac9-132">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="1fac9-133">响应</span><span class="sxs-lookup"><span data-stu-id="1fac9-133">Response</span></span>

<span data-ttu-id="1fac9-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fac9-134">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1fac9-135">示例</span><span class="sxs-lookup"><span data-stu-id="1fac9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fac9-136">请求</span><span class="sxs-lookup"><span data-stu-id="1fac9-136">Request</span></span>
<span data-ttu-id="1fac9-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1fac9-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fac9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fac9-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1fac9-139">C#</span><span class="sxs-lookup"><span data-stu-id="1fac9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fac9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fac9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fac9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fac9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1fac9-142">响应</span><span class="sxs-lookup"><span data-stu-id="1fac9-142">Response</span></span>
<span data-ttu-id="1fac9-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1fac9-143">Here is an example of the response.</span></span>
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
