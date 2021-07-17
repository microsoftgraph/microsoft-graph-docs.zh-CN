---
title: 创建 externalItem
description: 创建新的 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7939689cf113e709853e5da666d1479e600fe4cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467581"
---
# <a name="create-externalitem"></a><span data-ttu-id="b2bd3-103">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="b2bd3-103">Create externalItem</span></span>

<span data-ttu-id="b2bd3-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b2bd3-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2bd3-105">创建新的 [externalItem](../resources/externalconnectors-externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-105">Create a new [externalItem](../resources/externalconnectors-externalitem.md).</span></span>

<span data-ttu-id="b2bd3-106">此 API 可用于创建自定义项。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="b2bd3-107">包含 [externalConnection](../resources/externalconnectors-externalconnection.md) 的架构 [必须已](../resources/externalconnectors-schema.md) 注册相应类型。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-107">The containing [externalConnection](../resources/externalconnectors-externalconnection.md) must have a [schema](../resources/externalconnectors-schema.md) registered of the corresponding type.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2bd3-108">权限</span><span class="sxs-lookup"><span data-stu-id="b2bd3-108">Permissions</span></span>

<span data-ttu-id="b2bd3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2bd3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2bd3-111">Permission type</span></span>                        | <span data-ttu-id="b2bd3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2bd3-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2bd3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2bd3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2bd3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-114">Not supported.</span></span> |
| <span data-ttu-id="b2bd3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2bd3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2bd3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-116">Not supported.</span></span> |
| <span data-ttu-id="b2bd3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2bd3-117">Application</span></span>                            | <span data-ttu-id="b2bd3-118">ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2bd3-118">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2bd3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2bd3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="b2bd3-120">路径参数</span><span class="sxs-lookup"><span data-stu-id="b2bd3-120">Path parameters</span></span>

| <span data-ttu-id="b2bd3-121">参数</span><span class="sxs-lookup"><span data-stu-id="b2bd3-121">Parameter</span></span>     | <span data-ttu-id="b2bd3-122">类型</span><span class="sxs-lookup"><span data-stu-id="b2bd3-122">Type</span></span>   | <span data-ttu-id="b2bd3-123">说明</span><span class="sxs-lookup"><span data-stu-id="b2bd3-123">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="b2bd3-124">connection-id</span><span class="sxs-lookup"><span data-stu-id="b2bd3-124">connection-id</span></span> | <span data-ttu-id="b2bd3-125">string</span><span class="sxs-lookup"><span data-stu-id="b2bd3-125">string</span></span> | <span data-ttu-id="b2bd3-126">`id`包含[externalConnection 的 属性](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="b2bd3-126">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="b2bd3-127">item-id</span><span class="sxs-lookup"><span data-stu-id="b2bd3-127">item-id</span></span>       | <span data-ttu-id="b2bd3-128">string</span><span class="sxs-lookup"><span data-stu-id="b2bd3-128">string</span></span> | <span data-ttu-id="b2bd3-129">由开发人员提供的 `id` [externalItem 属性](../resources/externalconnectors-externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-129">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> <span data-ttu-id="b2bd3-130">如果不存在此项目，将 `id` 创建一个新项。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-130">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="b2bd3-131">如果项目已存在， `id` 则它将被正文中发送的对象覆盖。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-131">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b2bd3-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2bd3-132">Request headers</span></span>

| <span data-ttu-id="b2bd3-133">名称</span><span class="sxs-lookup"><span data-stu-id="b2bd3-133">Name</span></span>          | <span data-ttu-id="b2bd3-134">说明</span><span class="sxs-lookup"><span data-stu-id="b2bd3-134">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="b2bd3-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2bd3-135">Authorization</span></span> | <span data-ttu-id="b2bd3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b2bd3-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2bd3-138">Content-Type</span></span>  | <span data-ttu-id="b2bd3-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b2bd3-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2bd3-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2bd3-141">Request body</span></span>

<span data-ttu-id="b2bd3-142">在请求正文中，提供 [externalItem](../resources/externalconnectors-externalitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-142">In the request body, supply a JSON representation of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span> <span data-ttu-id="b2bd3-143">有效负载限制为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-143">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="b2bd3-144">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="b2bd3-144">Creating an externalItem</span></span>

<span data-ttu-id="b2bd3-145">创建 时 `externalItem` ，以下字段是必需的： `acl` 和 `properties` 。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-145">When creating an `externalItem`, the following fields are required: `acl`, and `properties`.</span></span> <span data-ttu-id="b2bd3-146">`properties`对象必须至少包含一个属性。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-146">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="b2bd3-147">所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-147">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="b2bd3-148">在下列 `externalItem` 情况下，上的 属性应在有效负载中使用类型说明符：</span><span class="sxs-lookup"><span data-stu-id="b2bd3-148">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="b2bd3-149">对于 `String` 类型属性，如果值包含非 ASCII 字符。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-149">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="b2bd3-150">对于所有集合类型。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-150">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="b2bd3-151">当包含 类型的 属性 `Collection(DateTime)` 时，必须使用类型说明器 `Collection(DateTimeOffset)` 。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-151">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="b2bd3-152">响应</span><span class="sxs-lookup"><span data-stu-id="b2bd3-152">Response</span></span>

<span data-ttu-id="b2bd3-153">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-153">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b2bd3-154">示例</span><span class="sxs-lookup"><span data-stu-id="b2bd3-154">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="b2bd3-155">示例：创建自定义项</span><span class="sxs-lookup"><span data-stu-id="b2bd3-155">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="b2bd3-156">请求</span><span class="sxs-lookup"><span data-stu-id="b2bd3-156">Request</span></span>

<span data-ttu-id="b2bd3-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2bd3-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2bd3-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    },
    {
      "type": "group",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny",
      "identitySource": "external"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="b2bd3-159">C#</span><span class="sxs-lookup"><span data-stu-id="b2bd3-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2bd3-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2bd3-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2bd3-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2bd3-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="b2bd3-162">响应</span><span class="sxs-lookup"><span data-stu-id="b2bd3-162">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b2bd3-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2bd3-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
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
