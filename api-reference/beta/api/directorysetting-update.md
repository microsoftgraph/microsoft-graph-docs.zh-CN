---
title: 更新目录设置
description: 更新特定目录设置对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e37c5b6886b5432395a9d70344d50251f1689ee5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951659"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="f2694-103">更新目录设置</span><span class="sxs-lookup"><span data-stu-id="f2694-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2694-104">更新特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2694-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="f2694-105">**注意**：此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="f2694-105">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="f2694-106">此 API 的/v1.0 版本已重命名为*更新 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="f2694-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2694-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f2694-107">Permissions</span></span>
<span data-ttu-id="f2694-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2694-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2694-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2694-110">Permission type</span></span>      | <span data-ttu-id="f2694-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2694-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2694-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2694-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2694-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2694-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2694-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2694-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2694-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2694-115">Not supported.</span></span>    |
|<span data-ttu-id="f2694-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2694-116">Application</span></span> | <span data-ttu-id="f2694-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2694-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2694-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2694-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f2694-119">更新租户范围或组特定设置。</span><span class="sxs-lookup"><span data-stu-id="f2694-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f2694-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f2694-120">Optional request headers</span></span>
| <span data-ttu-id="f2694-121">名称</span><span class="sxs-lookup"><span data-stu-id="f2694-121">Name</span></span>       | <span data-ttu-id="f2694-122">说明</span><span class="sxs-lookup"><span data-stu-id="f2694-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f2694-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2694-123">Authorization</span></span>  | <span data-ttu-id="f2694-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2694-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2694-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2694-126">Request body</span></span>
<span data-ttu-id="f2694-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f2694-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="f2694-128">属性</span><span class="sxs-lookup"><span data-stu-id="f2694-128">Property</span></span>     | <span data-ttu-id="f2694-129">类型</span><span class="sxs-lookup"><span data-stu-id="f2694-129">Type</span></span>   |<span data-ttu-id="f2694-130">Description</span><span class="sxs-lookup"><span data-stu-id="f2694-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2694-131">值</span><span class="sxs-lookup"><span data-stu-id="f2694-131">values</span></span> | <span data-ttu-id="f2694-132">[settingValue](../resources/settingvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="f2694-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="f2694-p104">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="f2694-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="f2694-136">响应</span><span class="sxs-lookup"><span data-stu-id="f2694-136">Response</span></span>

<span data-ttu-id="f2694-137">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2694-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f2694-138">示例</span><span class="sxs-lookup"><span data-stu-id="f2694-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2694-139">请求</span><span class="sxs-lookup"><span data-stu-id="f2694-139">Request</span></span>
<span data-ttu-id="f2694-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2694-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f2694-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2694-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f2694-142">C#</span><span class="sxs-lookup"><span data-stu-id="f2694-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2694-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2694-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f2694-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2694-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f2694-145">响应</span><span class="sxs-lookup"><span data-stu-id="f2694-145">Response</span></span>
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
