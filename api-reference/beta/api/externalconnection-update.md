---
title: 更新 externalConnection
description: 更新 externalConnection 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6210d9b6cbd127eb4de28f72ac41972de5059c1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422045"
---
# <a name="update-connection"></a><span data-ttu-id="8ac83-103">更新连接</span><span class="sxs-lookup"><span data-stu-id="8ac83-103">Update connection</span></span>

<span data-ttu-id="8ac83-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8ac83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ac83-105">更新[externalConnection](../resources/externalconnection.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="8ac83-105">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="8ac83-106">权限</span><span class="sxs-lookup"><span data-stu-id="8ac83-106">Permissions</span></span>

<span data-ttu-id="8ac83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ac83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ac83-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ac83-109">Permission type</span></span>                        | <span data-ttu-id="8ac83-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ac83-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ac83-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ac83-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ac83-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ac83-112">Not supported.</span></span> |
| <span data-ttu-id="8ac83-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ac83-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ac83-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ac83-114">Not supported.</span></span> |
| <span data-ttu-id="8ac83-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ac83-115">Application</span></span>                            | <span data-ttu-id="8ac83-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ac83-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ac83-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ac83-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ac83-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ac83-118">Request headers</span></span>

| <span data-ttu-id="8ac83-119">名称</span><span class="sxs-lookup"><span data-stu-id="8ac83-119">Name</span></span>          | <span data-ttu-id="8ac83-120">说明</span><span class="sxs-lookup"><span data-stu-id="8ac83-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="8ac83-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ac83-121">Authorization</span></span> | <span data-ttu-id="8ac83-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ac83-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8ac83-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ac83-124">Content-Type</span></span>  | <span data-ttu-id="8ac83-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8ac83-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ac83-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ac83-127">Request body</span></span>

<span data-ttu-id="8ac83-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8ac83-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8ac83-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8ac83-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8ac83-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8ac83-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="8ac83-131">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="8ac83-131">The following properties can be updated.</span></span>

| <span data-ttu-id="8ac83-132">属性</span><span class="sxs-lookup"><span data-stu-id="8ac83-132">Property</span></span>      | <span data-ttu-id="8ac83-133">类型</span><span class="sxs-lookup"><span data-stu-id="8ac83-133">Type</span></span>                                           | <span data-ttu-id="8ac83-134">说明</span><span class="sxs-lookup"><span data-stu-id="8ac83-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="8ac83-135">设置</span><span class="sxs-lookup"><span data-stu-id="8ac83-135">configuration</span></span> | [<span data-ttu-id="8ac83-136">configuration</span><span class="sxs-lookup"><span data-stu-id="8ac83-136">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="8ac83-137">指定允许管理连接和索引连接中的内容的其他应用程序 Id。</span><span class="sxs-lookup"><span data-stu-id="8ac83-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="8ac83-138">说明</span><span class="sxs-lookup"><span data-stu-id="8ac83-138">description</span></span>   | <span data-ttu-id="8ac83-139">String</span><span class="sxs-lookup"><span data-stu-id="8ac83-139">String</span></span>                                         | <span data-ttu-id="8ac83-140">Microsoft 365 管理中心显示的连接的说明。</span><span class="sxs-lookup"><span data-stu-id="8ac83-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="8ac83-141">name</span><span class="sxs-lookup"><span data-stu-id="8ac83-141">name</span></span>          | <span data-ttu-id="8ac83-142">String</span><span class="sxs-lookup"><span data-stu-id="8ac83-142">String</span></span>                                         | <span data-ttu-id="8ac83-143">要显示在 Microsoft 365 管理中心中的连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8ac83-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="8ac83-144">最大长度为128个字符。</span><span class="sxs-lookup"><span data-stu-id="8ac83-144">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="8ac83-145">响应</span><span class="sxs-lookup"><span data-stu-id="8ac83-145">Response</span></span>

<span data-ttu-id="8ac83-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8ac83-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8ac83-147">示例</span><span class="sxs-lookup"><span data-stu-id="8ac83-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ac83-148">请求</span><span class="sxs-lookup"><span data-stu-id="8ac83-148">Request</span></span>

<span data-ttu-id="8ac83-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8ac83-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ac83-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ac83-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8ac83-151">C#</span><span class="sxs-lookup"><span data-stu-id="8ac83-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ac83-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ac83-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ac83-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ac83-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8ac83-154">响应</span><span class="sxs-lookup"><span data-stu-id="8ac83-154">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="8ac83-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8ac83-155">The following is an example of the response.</span></span>

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
