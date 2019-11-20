---
title: 更新 externalConnection
description: 更新 externalConnection 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 33dd46c03056026337713b35197be5a65ed17485
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747200"
---
# <a name="update-connection"></a><span data-ttu-id="99783-103">更新连接</span><span class="sxs-lookup"><span data-stu-id="99783-103">Update connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99783-104">更新[externalConnection](../resources/externalconnection.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="99783-104">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="99783-105">权限</span><span class="sxs-lookup"><span data-stu-id="99783-105">Permissions</span></span>

<span data-ttu-id="99783-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99783-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="99783-108">Permission type</span></span>                        | <span data-ttu-id="99783-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99783-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="99783-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99783-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="99783-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="99783-111">Not supported.</span></span> |
| <span data-ttu-id="99783-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99783-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99783-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="99783-113">Not supported.</span></span> |
| <span data-ttu-id="99783-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="99783-114">Application</span></span>                            | <span data-ttu-id="99783-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99783-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99783-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99783-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="99783-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="99783-117">Request headers</span></span>

| <span data-ttu-id="99783-118">名称</span><span class="sxs-lookup"><span data-stu-id="99783-118">Name</span></span>          | <span data-ttu-id="99783-119">说明</span><span class="sxs-lookup"><span data-stu-id="99783-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="99783-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="99783-120">Authorization</span></span> | <span data-ttu-id="99783-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99783-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="99783-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99783-123">Content-Type</span></span>  | <span data-ttu-id="99783-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="99783-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99783-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99783-126">Request body</span></span>

<span data-ttu-id="99783-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="99783-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="99783-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="99783-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="99783-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="99783-129">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="99783-130">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="99783-130">The following properties can be updated.</span></span>

| <span data-ttu-id="99783-131">属性</span><span class="sxs-lookup"><span data-stu-id="99783-131">Property</span></span>      | <span data-ttu-id="99783-132">类型</span><span class="sxs-lookup"><span data-stu-id="99783-132">Type</span></span>                                           | <span data-ttu-id="99783-133">说明</span><span class="sxs-lookup"><span data-stu-id="99783-133">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="99783-134">设置</span><span class="sxs-lookup"><span data-stu-id="99783-134">configuration</span></span> | [<span data-ttu-id="99783-135">configuration</span><span class="sxs-lookup"><span data-stu-id="99783-135">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="99783-136">指定允许管理连接和索引连接中的内容的其他应用程序 Id。</span><span class="sxs-lookup"><span data-stu-id="99783-136">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="99783-137">说明</span><span class="sxs-lookup"><span data-stu-id="99783-137">description</span></span>   | <span data-ttu-id="99783-138">String</span><span class="sxs-lookup"><span data-stu-id="99783-138">String</span></span>                                         | <span data-ttu-id="99783-139">Microsoft 365 管理中心显示的连接的说明。</span><span class="sxs-lookup"><span data-stu-id="99783-139">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="99783-140">name</span><span class="sxs-lookup"><span data-stu-id="99783-140">name</span></span>          | <span data-ttu-id="99783-141">String</span><span class="sxs-lookup"><span data-stu-id="99783-141">String</span></span>                                         | <span data-ttu-id="99783-142">要显示在 Microsoft 365 管理中心中的连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="99783-142">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="99783-143">最大长度为128个字符。</span><span class="sxs-lookup"><span data-stu-id="99783-143">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="99783-144">响应</span><span class="sxs-lookup"><span data-stu-id="99783-144">Response</span></span>

<span data-ttu-id="99783-145">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="99783-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="99783-146">示例</span><span class="sxs-lookup"><span data-stu-id="99783-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99783-147">请求</span><span class="sxs-lookup"><span data-stu-id="99783-147">Request</span></span>

<span data-ttu-id="99783-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99783-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99783-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="99783-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connection"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99783-150">C#</span><span class="sxs-lookup"><span data-stu-id="99783-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99783-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99783-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99783-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99783-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="99783-153">响应</span><span class="sxs-lookup"><span data-stu-id="99783-153">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="99783-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99783-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
