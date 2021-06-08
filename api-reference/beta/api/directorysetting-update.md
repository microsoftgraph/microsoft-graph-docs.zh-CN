---
title: 更新目录设置
description: 更新特定目录设置对象的属性。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 08f6c51413f751a0ce5a2818969e253d32f5e2fe
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786830"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="39811-103">更新目录设置</span><span class="sxs-lookup"><span data-stu-id="39811-103">Update a directory setting</span></span>

<span data-ttu-id="39811-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39811-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39811-105">更新特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="39811-105">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="39811-106">**注意**：此 API 的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="39811-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="39811-107">此 API 的 /v1.0 版本已重命名为 *Update groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="39811-107">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="39811-108">权限</span><span class="sxs-lookup"><span data-stu-id="39811-108">Permissions</span></span>
<span data-ttu-id="39811-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39811-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39811-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39811-111">Permission type</span></span>      | <span data-ttu-id="39811-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39811-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39811-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39811-113">Delegated (work or school account)</span></span> | <span data-ttu-id="39811-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39811-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39811-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39811-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39811-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="39811-116">Not supported.</span></span>    |
|<span data-ttu-id="39811-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39811-117">Application</span></span> | <span data-ttu-id="39811-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39811-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39811-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39811-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="39811-120">更新租户范围或组特定设置。</span><span class="sxs-lookup"><span data-stu-id="39811-120">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="39811-121">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="39811-121">Optional request headers</span></span>
| <span data-ttu-id="39811-122">名称</span><span class="sxs-lookup"><span data-stu-id="39811-122">Name</span></span>       | <span data-ttu-id="39811-123">说明</span><span class="sxs-lookup"><span data-stu-id="39811-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="39811-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="39811-124">Authorization</span></span>  | <span data-ttu-id="39811-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39811-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39811-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="39811-127">Request body</span></span>
<span data-ttu-id="39811-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="39811-128">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="39811-129">属性</span><span class="sxs-lookup"><span data-stu-id="39811-129">Property</span></span>     | <span data-ttu-id="39811-130">类型</span><span class="sxs-lookup"><span data-stu-id="39811-130">Type</span></span>   |<span data-ttu-id="39811-131">说明</span><span class="sxs-lookup"><span data-stu-id="39811-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="39811-132">值</span><span class="sxs-lookup"><span data-stu-id="39811-132">values</span></span> | <span data-ttu-id="39811-133">[settingValue](../resources/settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39811-133">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="39811-p104">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="39811-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="39811-137">响应</span><span class="sxs-lookup"><span data-stu-id="39811-137">Response</span></span>

<span data-ttu-id="39811-138">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="39811-138">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39811-139">示例</span><span class="sxs-lookup"><span data-stu-id="39811-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39811-140">请求</span><span class="sxs-lookup"><span data-stu-id="39811-140">Request</span></span>
<span data-ttu-id="39811-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39811-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39811-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="39811-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="39811-143">C#</span><span class="sxs-lookup"><span data-stu-id="39811-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39811-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39811-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39811-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39811-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39811-146">Java</span><span class="sxs-lookup"><span data-stu-id="39811-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="39811-147">响应</span><span class="sxs-lookup"><span data-stu-id="39811-147">Response</span></span>
<!-- {
  "blockType": "response"
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


