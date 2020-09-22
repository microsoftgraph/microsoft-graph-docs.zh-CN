---
title: 创建架构
description: 为 Microsoft Search 连接创建架构。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b26239d3f669b345a19591b01a2139c4101c3768
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006844"
---
# <a name="create-schema"></a><span data-ttu-id="db82c-103">创建架构</span><span class="sxs-lookup"><span data-stu-id="db82c-103">Create schema</span></span>

<span data-ttu-id="db82c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db82c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db82c-105">为 Microsoft Search [连接](../resources/externalconnection.md)创建架构。</span><span class="sxs-lookup"><span data-stu-id="db82c-105">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="db82c-106">权限</span><span class="sxs-lookup"><span data-stu-id="db82c-106">Permissions</span></span>

<span data-ttu-id="db82c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db82c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db82c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db82c-109">Permission type</span></span>                        | <span data-ttu-id="db82c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db82c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db82c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db82c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db82c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="db82c-112">Not supported.</span></span> |
| <span data-ttu-id="db82c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db82c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db82c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db82c-114">Not supported.</span></span> |
| <span data-ttu-id="db82c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db82c-115">Application</span></span>                            | <span data-ttu-id="db82c-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db82c-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db82c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db82c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="db82c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db82c-118">Request headers</span></span>

| <span data-ttu-id="db82c-119">名称</span><span class="sxs-lookup"><span data-stu-id="db82c-119">Name</span></span>                  | <span data-ttu-id="db82c-120">说明</span><span class="sxs-lookup"><span data-stu-id="db82c-120">Description</span></span>                                                        |
|:----------------------|:-------------------------------------------------------------------|
| <span data-ttu-id="db82c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db82c-121">Authorization</span></span>         | <span data-ttu-id="db82c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db82c-p102">Bearer {token}. Required.</span></span>                                          |
| <span data-ttu-id="db82c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db82c-124">Content-Type</span></span>          | <span data-ttu-id="db82c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="db82c-p103">application/json. Required.</span></span>                                        |
| <span data-ttu-id="db82c-127">首选：响应-async</span><span class="sxs-lookup"><span data-stu-id="db82c-127">Prefer: respond-async</span></span> | <span data-ttu-id="db82c-128">使用此来导致请求以异步方式执行。</span><span class="sxs-lookup"><span data-stu-id="db82c-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="db82c-129">可选。</span><span class="sxs-lookup"><span data-stu-id="db82c-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db82c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="db82c-130">Request body</span></span>

<span data-ttu-id="db82c-131">在请求正文中，提供 [架构](../resources/schema.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db82c-131">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="db82c-132">注册自定义项目架构时， `schema` 对象的 `baseType` 属性必须设置为 `microsoft.graph.externalItem` ，并且必须包含 `properties` 属性。</span><span class="sxs-lookup"><span data-stu-id="db82c-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="db82c-133">该 `properties` 对象必须至少包含一个属性，最多为64。</span><span class="sxs-lookup"><span data-stu-id="db82c-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="db82c-134">响应</span><span class="sxs-lookup"><span data-stu-id="db82c-134">Response</span></span>

<span data-ttu-id="db82c-135">在 `Prefer: respond-async` 请求中包含标头的情况下，如果成功，此方法将在 `202 Accepted` 响应标头中返回响应代码和 URL， `Location` 该 URL 可用于 [获取操作状态](../api/connectionoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="db82c-135">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="db82c-136">如果在 `Prefer: respond-async` 请求中不包含标头，则此方法在 `201 Created` 响应正文中返回响应代码和新 [架构](../resources/schema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db82c-136">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="db82c-137">创建架构是一个容易导致网关超时的长时间运行的过程。</span><span class="sxs-lookup"><span data-stu-id="db82c-137">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="db82c-138">我们建议使用 `Prefer: respond-async` 标头以避免超时错误。</span><span class="sxs-lookup"><span data-stu-id="db82c-138">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="db82c-139">示例</span><span class="sxs-lookup"><span data-stu-id="db82c-139">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="db82c-140">示例：异步注册自定义架构</span><span class="sxs-lookup"><span data-stu-id="db82c-140">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="db82c-141">请求</span><span class="sxs-lookup"><span data-stu-id="db82c-141">Request</span></span>

<span data-ttu-id="db82c-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db82c-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db82c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="db82c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="db82c-144">C#</span><span class="sxs-lookup"><span data-stu-id="db82c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db82c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db82c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db82c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db82c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="db82c-147">响应</span><span class="sxs-lookup"><span data-stu-id="db82c-147">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="db82c-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db82c-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
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


