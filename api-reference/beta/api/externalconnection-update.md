---
title: 更新 externalConnection
description: 更新 externalConnection 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f6de3acfbdc71a83e087c58f11b8d93d7fbc5452
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366785"
---
# <a name="update-connection"></a><span data-ttu-id="b603f-103">更新连接</span><span class="sxs-lookup"><span data-stu-id="b603f-103">Update connection</span></span>

<span data-ttu-id="b603f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b603f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b603f-105">更新 [externalConnection 的属性](../resources/externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="b603f-105">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b603f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b603f-106">Permissions</span></span>

<span data-ttu-id="b603f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b603f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b603f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b603f-109">Permission type</span></span>                        | <span data-ttu-id="b603f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b603f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b603f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b603f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b603f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b603f-112">Not supported.</span></span> |
| <span data-ttu-id="b603f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b603f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b603f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b603f-114">Not supported.</span></span> |
| <span data-ttu-id="b603f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b603f-115">Application</span></span>                            | <span data-ttu-id="b603f-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b603f-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b603f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b603f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b603f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b603f-118">Request headers</span></span>

| <span data-ttu-id="b603f-119">名称</span><span class="sxs-lookup"><span data-stu-id="b603f-119">Name</span></span>          | <span data-ttu-id="b603f-120">说明</span><span class="sxs-lookup"><span data-stu-id="b603f-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="b603f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b603f-121">Authorization</span></span> | <span data-ttu-id="b603f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b603f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b603f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b603f-124">Content-Type</span></span>  | <span data-ttu-id="b603f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b603f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b603f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b603f-127">Request body</span></span>

<span data-ttu-id="b603f-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b603f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b603f-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b603f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b603f-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b603f-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="b603f-131">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="b603f-131">The following properties can be updated.</span></span>

| <span data-ttu-id="b603f-132">属性</span><span class="sxs-lookup"><span data-stu-id="b603f-132">Property</span></span>      | <span data-ttu-id="b603f-133">类型</span><span class="sxs-lookup"><span data-stu-id="b603f-133">Type</span></span>                                           | <span data-ttu-id="b603f-134">说明</span><span class="sxs-lookup"><span data-stu-id="b603f-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="b603f-135">configuration</span><span class="sxs-lookup"><span data-stu-id="b603f-135">configuration</span></span> | [<span data-ttu-id="b603f-136">configuration</span><span class="sxs-lookup"><span data-stu-id="b603f-136">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="b603f-137">指定允许管理连接和索引连接内容的其他应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="b603f-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="b603f-138">说明</span><span class="sxs-lookup"><span data-stu-id="b603f-138">description</span></span>   | <span data-ttu-id="b603f-139">String</span><span class="sxs-lookup"><span data-stu-id="b603f-139">String</span></span>                                         | <span data-ttu-id="b603f-140">网站中显示的连接Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="b603f-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="b603f-141">name</span><span class="sxs-lookup"><span data-stu-id="b603f-141">name</span></span>          | <span data-ttu-id="b603f-142">String</span><span class="sxs-lookup"><span data-stu-id="b603f-142">String</span></span>                                         | <span data-ttu-id="b603f-143">要显示名称中显示的连接的Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="b603f-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="b603f-144">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="b603f-144">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="b603f-145">响应</span><span class="sxs-lookup"><span data-stu-id="b603f-145">Response</span></span>

<span data-ttu-id="b603f-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b603f-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b603f-147">示例</span><span class="sxs-lookup"><span data-stu-id="b603f-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b603f-148">请求</span><span class="sxs-lookup"><span data-stu-id="b603f-148">Request</span></span>

<span data-ttu-id="b603f-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b603f-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b603f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="b603f-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b603f-151">C#</span><span class="sxs-lookup"><span data-stu-id="b603f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b603f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b603f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b603f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b603f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b603f-154">Java</span><span class="sxs-lookup"><span data-stu-id="b603f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b603f-155">响应</span><span class="sxs-lookup"><span data-stu-id="b603f-155">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b603f-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b603f-156">The following is an example of the response.</span></span>

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


