---
title: 更新目录设置
description: 更新特定目录设置对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b62044ad833d9d8f2e05d49e430d375654c766
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436753"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="9a532-103">更新目录设置</span><span class="sxs-lookup"><span data-stu-id="9a532-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a532-104">更新特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a532-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="9a532-105">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="9a532-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="9a532-106">此 API 的/v1.0 版本已重命名为*更新 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="9a532-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a532-107">权限</span><span class="sxs-lookup"><span data-stu-id="9a532-107">Permissions</span></span>
<span data-ttu-id="9a532-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a532-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a532-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a532-110">Permission type</span></span>      | <span data-ttu-id="9a532-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a532-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a532-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a532-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a532-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a532-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a532-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a532-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a532-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a532-115">Not supported.</span></span>    |
|<span data-ttu-id="9a532-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a532-116">Application</span></span> | <span data-ttu-id="9a532-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a532-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a532-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a532-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9a532-119">更新租户范围或组特定设置。</span><span class="sxs-lookup"><span data-stu-id="9a532-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="9a532-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="9a532-120">Optional request headers</span></span>
| <span data-ttu-id="9a532-121">名称</span><span class="sxs-lookup"><span data-stu-id="9a532-121">Name</span></span>       | <span data-ttu-id="9a532-122">说明</span><span class="sxs-lookup"><span data-stu-id="9a532-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a532-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a532-123">Authorization</span></span>  | <span data-ttu-id="9a532-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a532-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a532-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a532-126">Request body</span></span>
<span data-ttu-id="9a532-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9a532-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="9a532-128">属性</span><span class="sxs-lookup"><span data-stu-id="9a532-128">Property</span></span>     | <span data-ttu-id="9a532-129">类型</span><span class="sxs-lookup"><span data-stu-id="9a532-129">Type</span></span>   |<span data-ttu-id="9a532-130">说明</span><span class="sxs-lookup"><span data-stu-id="9a532-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a532-131">值</span><span class="sxs-lookup"><span data-stu-id="9a532-131">values</span></span> | <span data-ttu-id="9a532-132">[settingValue](../resources/settingvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a532-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="9a532-p104">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="9a532-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="9a532-136">响应</span><span class="sxs-lookup"><span data-stu-id="9a532-136">Response</span></span>

<span data-ttu-id="9a532-137">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9a532-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9a532-138">示例</span><span class="sxs-lookup"><span data-stu-id="9a532-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a532-139">请求</span><span class="sxs-lookup"><span data-stu-id="9a532-139">Request</span></span>
<span data-ttu-id="9a532-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a532-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a532-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9a532-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a532-142">C#</span><span class="sxs-lookup"><span data-stu-id="9a532-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a532-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a532-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a532-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="9a532-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a532-145">响应</span><span class="sxs-lookup"><span data-stu-id="9a532-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
