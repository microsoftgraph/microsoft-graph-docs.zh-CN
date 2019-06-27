---
title: 更新目录设置
description: 更新特定目录设置对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 65519a4bd4ae9e4640ec3d5b3abc604096bcd4b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260534"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="f9558-103">更新目录设置</span><span class="sxs-lookup"><span data-stu-id="f9558-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9558-104">更新特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9558-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="f9558-105">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="f9558-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f9558-106">此 API 的/v1.0 版本已重命名为*更新 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="f9558-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9558-107">权限</span><span class="sxs-lookup"><span data-stu-id="f9558-107">Permissions</span></span>
<span data-ttu-id="f9558-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9558-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9558-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9558-110">Permission type</span></span>      | <span data-ttu-id="f9558-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9558-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9558-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9558-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9558-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9558-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9558-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9558-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9558-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9558-115">Not supported.</span></span>    |
|<span data-ttu-id="f9558-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9558-116">Application</span></span> | <span data-ttu-id="f9558-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9558-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9558-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9558-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f9558-119">更新租户范围或组特定设置。</span><span class="sxs-lookup"><span data-stu-id="f9558-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f9558-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f9558-120">Optional request headers</span></span>
| <span data-ttu-id="f9558-121">名称</span><span class="sxs-lookup"><span data-stu-id="f9558-121">Name</span></span>       | <span data-ttu-id="f9558-122">说明</span><span class="sxs-lookup"><span data-stu-id="f9558-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f9558-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9558-123">Authorization</span></span>  | <span data-ttu-id="f9558-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9558-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9558-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9558-126">Request body</span></span>
<span data-ttu-id="f9558-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f9558-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="f9558-128">属性</span><span class="sxs-lookup"><span data-stu-id="f9558-128">Property</span></span>     | <span data-ttu-id="f9558-129">类型</span><span class="sxs-lookup"><span data-stu-id="f9558-129">Type</span></span>   |<span data-ttu-id="f9558-130">说明</span><span class="sxs-lookup"><span data-stu-id="f9558-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9558-131">值</span><span class="sxs-lookup"><span data-stu-id="f9558-131">values</span></span> | <span data-ttu-id="f9558-132">[settingValue](../resources/settingvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9558-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="f9558-p104">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="f9558-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="f9558-136">响应</span><span class="sxs-lookup"><span data-stu-id="f9558-136">Response</span></span>

<span data-ttu-id="f9558-137">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f9558-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9558-138">示例</span><span class="sxs-lookup"><span data-stu-id="f9558-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9558-139">请求</span><span class="sxs-lookup"><span data-stu-id="f9558-139">Request</span></span>
<span data-ttu-id="f9558-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9558-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f9558-141">响应</span><span class="sxs-lookup"><span data-stu-id="f9558-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f9558-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f9558-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f9558-143">C#</span><span class="sxs-lookup"><span data-stu-id="f9558-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9558-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9558-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_directorysetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f9558-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="f9558-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_directorysetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
