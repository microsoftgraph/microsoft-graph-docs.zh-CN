---
title: 创建架构
description: 为 Microsoft Search 连接创建架构。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7fd9a9caa8c85df45fb292f822a7a1959175316b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422143"
---
# <a name="create-schema"></a><span data-ttu-id="d794a-103">创建架构</span><span class="sxs-lookup"><span data-stu-id="d794a-103">Create schema</span></span>

<span data-ttu-id="d794a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d794a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d794a-105">为 Microsoft Search[连接](../resources/externalconnection.md)创建架构。</span><span class="sxs-lookup"><span data-stu-id="d794a-105">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

<span data-ttu-id="d794a-106">支持两种架构类型：自定义项和文件。</span><span class="sxs-lookup"><span data-stu-id="d794a-106">Two schema types are supported: custom items, and files.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="d794a-107">权限</span><span class="sxs-lookup"><span data-stu-id="d794a-107">Permissions</span></span>

<span data-ttu-id="d794a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d794a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d794a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d794a-110">Permission type</span></span>                        | <span data-ttu-id="d794a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d794a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d794a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d794a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d794a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d794a-113">Not supported.</span></span> |
| <span data-ttu-id="d794a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d794a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d794a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d794a-115">Not supported.</span></span> |
| <span data-ttu-id="d794a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d794a-116">Application</span></span>                            | <span data-ttu-id="d794a-117">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d794a-117">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d794a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d794a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="d794a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d794a-119">Request headers</span></span>

| <span data-ttu-id="d794a-120">名称</span><span class="sxs-lookup"><span data-stu-id="d794a-120">Name</span></span>                  | <span data-ttu-id="d794a-121">说明</span><span class="sxs-lookup"><span data-stu-id="d794a-121">Description</span></span>                                          |
|:----------------------|:-----------------------------------------------------|
| <span data-ttu-id="d794a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d794a-122">Authorization</span></span>         | <span data-ttu-id="d794a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d794a-p102">Bearer {token}. Required.</span></span>                            |
| <span data-ttu-id="d794a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d794a-125">Content-Type</span></span>          | <span data-ttu-id="d794a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d794a-p103">application/json. Required.</span></span>                          |
| <span data-ttu-id="d794a-128">首选：响应-async</span><span class="sxs-lookup"><span data-stu-id="d794a-128">Prefer: respond-async</span></span> | <span data-ttu-id="d794a-129">使用此来导致请求以异步方式执行。</span><span class="sxs-lookup"><span data-stu-id="d794a-129">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="d794a-130">可选。</span><span class="sxs-lookup"><span data-stu-id="d794a-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d794a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d794a-131">Request body</span></span>

<span data-ttu-id="d794a-132">在请求正文中，提供[架构](../resources/schema.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d794a-132">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="d794a-133">注册自`schema`定义项目架构时，对象的`baseType`属性必须设置为`microsoft.graph.externalItem` ，并且必须包含`properties`属性。</span><span class="sxs-lookup"><span data-stu-id="d794a-133">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="d794a-134">该`properties`对象必须至少包含一个属性，最多为64。</span><span class="sxs-lookup"><span data-stu-id="d794a-134">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

<span data-ttu-id="d794a-135">注册文件架构时， `schema`对象的`baseType`属性必须设置为。 `microsoft.graph.externalFile`</span><span class="sxs-lookup"><span data-stu-id="d794a-135">When registering a file schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalFile`.</span></span>

## <a name="response"></a><span data-ttu-id="d794a-136">响应</span><span class="sxs-lookup"><span data-stu-id="d794a-136">Response</span></span>

<span data-ttu-id="d794a-137">在请求`Prefer: respond-async`中包含标头的情况下，如果成功，此方法`202 Accepted`将在`Location`响应标头中返回响应代码和 URL，该 URL 可用于[获取操作状态](../api/connectionoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="d794a-137">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="d794a-138">如果在`Prefer: respond-async`请求中不包含标头，则此方法在响应正文`201 Created`中返回响应代码和新[架构](../resources/schema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d794a-138">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="d794a-139">创建架构是一个容易导致网关超时的长时间运行的过程。</span><span class="sxs-lookup"><span data-stu-id="d794a-139">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="d794a-140">我们建议使用`Prefer: respond-async`标头以避免超时错误。</span><span class="sxs-lookup"><span data-stu-id="d794a-140">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="d794a-141">示例</span><span class="sxs-lookup"><span data-stu-id="d794a-141">Examples</span></span>

### <a name="example-1-register-custom-schema-asynchronously"></a><span data-ttu-id="d794a-142">示例1：异步注册自定义架构</span><span class="sxs-lookup"><span data-stu-id="d794a-142">Example 1: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="d794a-143">请求</span><span class="sxs-lookup"><span data-stu-id="d794a-143">Request</span></span>

<span data-ttu-id="d794a-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d794a-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d794a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d794a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "title",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d794a-146">C#</span><span class="sxs-lookup"><span data-stu-id="d794a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d794a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d794a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d794a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d794a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="d794a-149">响应</span><span class="sxs-lookup"><span data-stu-id="d794a-149">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d794a-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d794a-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

### <a name="example-2-register-file-schema-synchronously"></a><span data-ttu-id="d794a-151">示例2：同步注册文件架构</span><span class="sxs-lookup"><span data-stu-id="d794a-151">Example 2: Register file schema synchronously</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="d794a-152">请求</span><span class="sxs-lookup"><span data-stu-id="d794a-152">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d794a-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d794a-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d794a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="d794a-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosofiles/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalFile"
}
```
# <a name="c"></a>[<span data-ttu-id="d794a-155">C#</span><span class="sxs-lookup"><span data-stu-id="d794a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d794a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d794a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d794a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d794a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="d794a-158">响应</span><span class="sxs-lookup"><span data-stu-id="d794a-158">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d794a-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d794a-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 201 Created

{
  "baseType": "microsoft.graph.externalFile"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
