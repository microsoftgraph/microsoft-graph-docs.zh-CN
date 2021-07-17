---
title: 创建架构
description: 为连接创建Microsoft 搜索架构。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b89fdd9ec7785639526f02344c8b4c7bc43335b1
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467582"
---
# <a name="create-schema"></a><span data-ttu-id="de3e8-103">创建架构</span><span class="sxs-lookup"><span data-stu-id="de3e8-103">Create schema</span></span>

<span data-ttu-id="de3e8-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="de3e8-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de3e8-105">为连接创建Microsoft 搜索[架构](../resources/externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="de3e8-105">Create the schema for a Microsoft Search [connection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="de3e8-106">权限</span><span class="sxs-lookup"><span data-stu-id="de3e8-106">Permissions</span></span>

<span data-ttu-id="de3e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de3e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de3e8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="de3e8-109">Permission type</span></span>                        | <span data-ttu-id="de3e8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de3e8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de3e8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de3e8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de3e8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="de3e8-112">Not supported.</span></span> |
| <span data-ttu-id="de3e8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de3e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de3e8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="de3e8-114">Not supported.</span></span> |
| <span data-ttu-id="de3e8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="de3e8-115">Application</span></span>                            | <span data-ttu-id="de3e8-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="de3e8-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="de3e8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de3e8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="de3e8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="de3e8-118">Request headers</span></span>

| <span data-ttu-id="de3e8-119">名称</span><span class="sxs-lookup"><span data-stu-id="de3e8-119">Name</span></span>                  | <span data-ttu-id="de3e8-120">说明</span><span class="sxs-lookup"><span data-stu-id="de3e8-120">Description</span></span>                                                        |
|:----------------------|:-------------------------------------------------------------------|
| <span data-ttu-id="de3e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de3e8-121">Authorization</span></span>         | <span data-ttu-id="de3e8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de3e8-p102">Bearer {token}. Required.</span></span>                                          |
| <span data-ttu-id="de3e8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de3e8-124">Content-Type</span></span>          | <span data-ttu-id="de3e8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="de3e8-p103">application/json. Required.</span></span>                                        |
| <span data-ttu-id="de3e8-127">Prefer：respond-async</span><span class="sxs-lookup"><span data-stu-id="de3e8-127">Prefer: respond-async</span></span> | <span data-ttu-id="de3e8-128">使用它会导致请求异步执行。</span><span class="sxs-lookup"><span data-stu-id="de3e8-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="de3e8-129">可选。</span><span class="sxs-lookup"><span data-stu-id="de3e8-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de3e8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="de3e8-130">Request body</span></span>

<span data-ttu-id="de3e8-131">在请求正文中，提供架构对象的 JSON [表示](../resources/externalconnectors-schema.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="de3e8-131">In the request body, supply a JSON representation of a [schema](../resources/externalconnectors-schema.md) object.</span></span>

<span data-ttu-id="de3e8-132">注册自定义项架构时， `schema` 对象必须将 `baseType` 属性设置为 `microsoft.graph.externalItem` ，并且必须包含 `properties` 属性。</span><span class="sxs-lookup"><span data-stu-id="de3e8-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="de3e8-133">`properties`对象必须至少包含一个属性，最多包含 64 个属性。</span><span class="sxs-lookup"><span data-stu-id="de3e8-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="de3e8-134">响应</span><span class="sxs-lookup"><span data-stu-id="de3e8-134">Response</span></span>

<span data-ttu-id="de3e8-135">在请求中包含 标头后，如果成功，此方法在响应标头中返回 响应代码和 `Prefer: respond-async` `202 Accepted` URL，可用于 `Location` [获取操作状态](../api/externalconnectors-connectionoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="de3e8-135">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/externalconnectors-connectionoperation-get.md).</span></span>

<span data-ttu-id="de3e8-136">如果请求中不包含 标头，如果成功，此方法在响应正文中返回 响应 `Prefer: respond-async` `201 Created` 代码和新[](../resources/externalconnectors-schema.md)架构对象。</span><span class="sxs-lookup"><span data-stu-id="de3e8-136">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="de3e8-137">创建架构是一个长时间运行的过程，容易出现网关超时。</span><span class="sxs-lookup"><span data-stu-id="de3e8-137">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="de3e8-138">我们建议使用 `Prefer: respond-async` 标头以避免超时错误。</span><span class="sxs-lookup"><span data-stu-id="de3e8-138">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="de3e8-139">示例</span><span class="sxs-lookup"><span data-stu-id="de3e8-139">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="de3e8-140">示例：异步注册自定义架构</span><span class="sxs-lookup"><span data-stu-id="de3e8-140">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="de3e8-141">请求</span><span class="sxs-lookup"><span data-stu-id="de3e8-141">Request</span></span>

<span data-ttu-id="de3e8-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="de3e8-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de3e8-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="de3e8-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
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
      "type": "string",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "string",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "string",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="de3e8-144">C#</span><span class="sxs-lookup"><span data-stu-id="de3e8-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de3e8-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de3e8-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de3e8-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de3e8-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de3e8-147">Java</span><span class="sxs-lookup"><span data-stu-id="de3e8-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schema-from-connection-async-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="de3e8-148">响应</span><span class="sxs-lookup"><span data-stu-id="de3e8-148">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="de3e8-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="de3e8-149">The following is an example of the response.</span></span>

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
