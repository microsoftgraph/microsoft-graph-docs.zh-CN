---
title: 创建架构
description: 为 Microsoft Search 连接创建架构。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: af5756277ddcf41a04ebed795ceeb4f1f0e3d08e
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892552"
---
# <a name="create-schema"></a><span data-ttu-id="69654-103">创建架构</span><span class="sxs-lookup"><span data-stu-id="69654-103">Create schema</span></span>

<span data-ttu-id="69654-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69654-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69654-105">为 Microsoft Search[连接](../resources/externalconnection.md)创建架构。</span><span class="sxs-lookup"><span data-stu-id="69654-105">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="69654-106">权限</span><span class="sxs-lookup"><span data-stu-id="69654-106">Permissions</span></span>

<span data-ttu-id="69654-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69654-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="69654-109">Permission type</span></span>                        | <span data-ttu-id="69654-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69654-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="69654-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69654-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="69654-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="69654-112">Not supported.</span></span> |
| <span data-ttu-id="69654-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69654-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69654-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="69654-114">Not supported.</span></span> |
| <span data-ttu-id="69654-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="69654-115">Application</span></span>                            | <span data-ttu-id="69654-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69654-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69654-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69654-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="69654-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="69654-118">Request headers</span></span>

| <span data-ttu-id="69654-119">名称</span><span class="sxs-lookup"><span data-stu-id="69654-119">Name</span></span>                  | <span data-ttu-id="69654-120">说明</span><span class="sxs-lookup"><span data-stu-id="69654-120">Description</span></span>                                                        |
|:----------------------|:-------------------------------------------------------------------|
| <span data-ttu-id="69654-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69654-121">Authorization</span></span>         | <span data-ttu-id="69654-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69654-p102">Bearer {token}. Required.</span></span>                                          |
| <span data-ttu-id="69654-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69654-124">Content-Type</span></span>          | <span data-ttu-id="69654-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="69654-p103">application/json. Required.</span></span>                                        |
| <span data-ttu-id="69654-127">首选：响应-async</span><span class="sxs-lookup"><span data-stu-id="69654-127">Prefer: respond-async</span></span> | <span data-ttu-id="69654-128">使用此来导致请求以异步方式执行。</span><span class="sxs-lookup"><span data-stu-id="69654-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="69654-129">可选。</span><span class="sxs-lookup"><span data-stu-id="69654-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69654-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="69654-130">Request body</span></span>

<span data-ttu-id="69654-131">在请求正文中，提供[架构](../resources/schema.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69654-131">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="69654-132">注册自`schema`定义项目架构时，对象的`baseType`属性必须设置为`microsoft.graph.externalItem` ，并且必须包含`properties`属性。</span><span class="sxs-lookup"><span data-stu-id="69654-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="69654-133">该`properties`对象必须至少包含一个属性，最多为64。</span><span class="sxs-lookup"><span data-stu-id="69654-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="69654-134">响应</span><span class="sxs-lookup"><span data-stu-id="69654-134">Response</span></span>

<span data-ttu-id="69654-135">在请求`Prefer: respond-async`中包含标头的情况下，如果成功，此方法`202 Accepted`将在`Location`响应标头中返回响应代码和 URL，该 URL 可用于[获取操作状态](../api/connectionoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="69654-135">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="69654-136">如果在`Prefer: respond-async`请求中不包含标头，则此方法在响应正文`201 Created`中返回响应代码和新[架构](../resources/schema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69654-136">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="69654-137">创建架构是一个容易导致网关超时的长时间运行的过程。</span><span class="sxs-lookup"><span data-stu-id="69654-137">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="69654-138">我们建议使用`Prefer: respond-async`标头以避免超时错误。</span><span class="sxs-lookup"><span data-stu-id="69654-138">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="69654-139">示例</span><span class="sxs-lookup"><span data-stu-id="69654-139">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="69654-140">示例：异步注册自定义架构</span><span class="sxs-lookup"><span data-stu-id="69654-140">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="69654-141">请求</span><span class="sxs-lookup"><span data-stu-id="69654-141">Request</span></span>

<span data-ttu-id="69654-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="69654-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69654-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="69654-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="69654-144">C#</span><span class="sxs-lookup"><span data-stu-id="69654-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69654-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69654-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69654-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69654-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="69654-147">响应</span><span class="sxs-lookup"><span data-stu-id="69654-147">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="69654-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="69654-148">The following is an example of the response.</span></span>

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
