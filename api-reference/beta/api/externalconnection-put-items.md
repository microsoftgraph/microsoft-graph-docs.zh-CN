---
title: 创建 externalItem
description: 创建新的 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: dfb3d3d6e10f2da9f1032aeeae0b6a2ba1c15087
ms.sourcegitcommit: c7c198f6fa252b68e91be341b93b818afd387486
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2020
ms.locfileid: "47439969"
---
# <a name="create-externalitem"></a><span data-ttu-id="50b18-103">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="50b18-103">Create externalItem</span></span>

<span data-ttu-id="50b18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50b18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50b18-105">创建新的 [externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="50b18-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="50b18-106">此 API 可用于创建自定义项。</span><span class="sxs-lookup"><span data-stu-id="50b18-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="50b18-107">通过在 JSON 正文中包含属性来指定要创建的类型 `@odata.type` 。</span><span class="sxs-lookup"><span data-stu-id="50b18-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="50b18-108">包含的 [externalConnection](../resources/externalconnection.md) 必须具有相应类型的已注册 [架构](../resources/schema.md) 。</span><span class="sxs-lookup"><span data-stu-id="50b18-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="50b18-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="50b18-109">Permissions</span></span>

<span data-ttu-id="50b18-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50b18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50b18-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="50b18-112">Permission type</span></span>                        | <span data-ttu-id="50b18-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50b18-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50b18-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50b18-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="50b18-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="50b18-115">Not supported.</span></span> |
| <span data-ttu-id="50b18-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50b18-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50b18-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="50b18-117">Not supported.</span></span> |
| <span data-ttu-id="50b18-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="50b18-118">Application</span></span>                            | <span data-ttu-id="50b18-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b18-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50b18-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50b18-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="50b18-121">路径参数</span><span class="sxs-lookup"><span data-stu-id="50b18-121">Path parameters</span></span>

| <span data-ttu-id="50b18-122">参数</span><span class="sxs-lookup"><span data-stu-id="50b18-122">Parameter</span></span>     | <span data-ttu-id="50b18-123">类型</span><span class="sxs-lookup"><span data-stu-id="50b18-123">Type</span></span>   | <span data-ttu-id="50b18-124">Description</span><span class="sxs-lookup"><span data-stu-id="50b18-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="50b18-125">connection-id</span><span class="sxs-lookup"><span data-stu-id="50b18-125">connection-id</span></span> | <span data-ttu-id="50b18-126">字符串</span><span class="sxs-lookup"><span data-stu-id="50b18-126">string</span></span> | <span data-ttu-id="50b18-127">`id`包含[externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="50b18-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="50b18-128">item-id</span><span class="sxs-lookup"><span data-stu-id="50b18-128">item-id</span></span>       | <span data-ttu-id="50b18-129">字符串</span><span class="sxs-lookup"><span data-stu-id="50b18-129">string</span></span> | <span data-ttu-id="50b18-130">ExternalItem 的开发人员提供的 `id` 属性[externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="50b18-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="50b18-131">如果不存在具有此项的项目 `id` ，则会创建一个新项目。</span><span class="sxs-lookup"><span data-stu-id="50b18-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="50b18-132">如果某个项目已经存在，则 `id` 会被在正文中发送的对象覆盖。</span><span class="sxs-lookup"><span data-stu-id="50b18-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="50b18-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="50b18-133">Request headers</span></span>

| <span data-ttu-id="50b18-134">名称</span><span class="sxs-lookup"><span data-stu-id="50b18-134">Name</span></span>          | <span data-ttu-id="50b18-135">说明</span><span class="sxs-lookup"><span data-stu-id="50b18-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="50b18-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b18-136">Authorization</span></span> | <span data-ttu-id="50b18-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50b18-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="50b18-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50b18-139">Content-Type</span></span>  | <span data-ttu-id="50b18-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50b18-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50b18-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="50b18-142">Request body</span></span>

<span data-ttu-id="50b18-143">在请求正文中，提供 [externalItem](../resources/externalitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50b18-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="50b18-144">有效负载限制为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="50b18-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="50b18-145">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="50b18-145">Creating an externalItem</span></span>

<span data-ttu-id="50b18-146">在创建时 `externalItem` ，需要以下字段： `@odata.type` 、 `acl` 和 `properties` 。</span><span class="sxs-lookup"><span data-stu-id="50b18-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="50b18-147">该 `properties` 对象必须至少包含一个属性。</span><span class="sxs-lookup"><span data-stu-id="50b18-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="50b18-148">所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="50b18-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="50b18-149">中的属性 `externalItem` 应在以下方案中使用有效负载中的类型说明符：</span><span class="sxs-lookup"><span data-stu-id="50b18-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="50b18-150">对于 `String` type 属性，如果该值包含非 ASCII 字符。</span><span class="sxs-lookup"><span data-stu-id="50b18-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="50b18-151">适用于所有集合类型。</span><span class="sxs-lookup"><span data-stu-id="50b18-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="50b18-152">如果包含类型的属性 `Collection(DateTime)` ，则必须使用类型说明符 `Collection(DateTimeOffset)` 。</span><span class="sxs-lookup"><span data-stu-id="50b18-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="50b18-153">响应</span><span class="sxs-lookup"><span data-stu-id="50b18-153">Response</span></span>

<span data-ttu-id="50b18-154">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="50b18-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="50b18-155">示例</span><span class="sxs-lookup"><span data-stu-id="50b18-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="50b18-156">示例：创建自定义项</span><span class="sxs-lookup"><span data-stu-id="50b18-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="50b18-157">请求</span><span class="sxs-lookup"><span data-stu-id="50b18-157">Request</span></span>

<span data-ttu-id="50b18-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="50b18-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50b18-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="50b18-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "deny",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="50b18-160">C#</span><span class="sxs-lookup"><span data-stu-id="50b18-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50b18-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50b18-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50b18-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50b18-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="50b18-163">响应</span><span class="sxs-lookup"><span data-stu-id="50b18-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="50b18-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="50b18-164">The following is an example of the response.</span></span>

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
