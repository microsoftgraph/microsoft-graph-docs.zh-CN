---
title: 创建 externalItem
description: 创建新的 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b4617596a10a85a4378b1e7ad4c4ca94fb16ffac
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491004"
---
# <a name="create-externalitem"></a><span data-ttu-id="2312f-103">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="2312f-103">Create externalItem</span></span>

<span data-ttu-id="2312f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2312f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2312f-105">创建新的 [externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="2312f-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="2312f-106">此 API 可用于创建自定义项。</span><span class="sxs-lookup"><span data-stu-id="2312f-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="2312f-107">在 JSON 正文中包括 属性 `@odata.type` ，指定要创建的类型。</span><span class="sxs-lookup"><span data-stu-id="2312f-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="2312f-108">包含 [externalConnection](../resources/externalconnection.md) 的架构 [必须已](../resources/schema.md) 注册相应类型。</span><span class="sxs-lookup"><span data-stu-id="2312f-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="2312f-109">权限</span><span class="sxs-lookup"><span data-stu-id="2312f-109">Permissions</span></span>

<span data-ttu-id="2312f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2312f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2312f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2312f-112">Permission type</span></span>                        | <span data-ttu-id="2312f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2312f-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2312f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2312f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2312f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2312f-115">Not supported.</span></span> |
| <span data-ttu-id="2312f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2312f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2312f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2312f-117">Not supported.</span></span> |
| <span data-ttu-id="2312f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="2312f-118">Application</span></span>                            | <span data-ttu-id="2312f-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2312f-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2312f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2312f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="2312f-121">路径参数</span><span class="sxs-lookup"><span data-stu-id="2312f-121">Path parameters</span></span>

| <span data-ttu-id="2312f-122">参数</span><span class="sxs-lookup"><span data-stu-id="2312f-122">Parameter</span></span>     | <span data-ttu-id="2312f-123">类型</span><span class="sxs-lookup"><span data-stu-id="2312f-123">Type</span></span>   | <span data-ttu-id="2312f-124">说明</span><span class="sxs-lookup"><span data-stu-id="2312f-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="2312f-125">connection-id</span><span class="sxs-lookup"><span data-stu-id="2312f-125">connection-id</span></span> | <span data-ttu-id="2312f-126">string</span><span class="sxs-lookup"><span data-stu-id="2312f-126">string</span></span> | <span data-ttu-id="2312f-127">`id`包含[externalConnection 的 属性](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="2312f-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="2312f-128">item-id</span><span class="sxs-lookup"><span data-stu-id="2312f-128">item-id</span></span>       | <span data-ttu-id="2312f-129">string</span><span class="sxs-lookup"><span data-stu-id="2312f-129">string</span></span> | <span data-ttu-id="2312f-130">由开发人员提供的 `id` [externalItem 属性](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="2312f-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="2312f-131">如果不存在此项目，将 `id` 创建一个新项。</span><span class="sxs-lookup"><span data-stu-id="2312f-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="2312f-132">如果项目已存在， `id` 则它将被正文中发送的对象覆盖。</span><span class="sxs-lookup"><span data-stu-id="2312f-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2312f-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="2312f-133">Request headers</span></span>

| <span data-ttu-id="2312f-134">名称</span><span class="sxs-lookup"><span data-stu-id="2312f-134">Name</span></span>          | <span data-ttu-id="2312f-135">说明</span><span class="sxs-lookup"><span data-stu-id="2312f-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="2312f-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="2312f-136">Authorization</span></span> | <span data-ttu-id="2312f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2312f-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2312f-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2312f-139">Content-Type</span></span>  | <span data-ttu-id="2312f-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2312f-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2312f-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="2312f-142">Request body</span></span>

<span data-ttu-id="2312f-143">在请求正文中，提供 [externalItem](../resources/externalitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2312f-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="2312f-144">有效负载限制为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="2312f-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="2312f-145">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="2312f-145">Creating an externalItem</span></span>

<span data-ttu-id="2312f-146">创建 时 `externalItem` ，以下字段是必需的 `@odata.type` ：、和 `acl` `properties` 。</span><span class="sxs-lookup"><span data-stu-id="2312f-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="2312f-147">`properties`对象必须至少包含一个属性。</span><span class="sxs-lookup"><span data-stu-id="2312f-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="2312f-148">所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="2312f-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="2312f-149">在下列 `externalItem` 情况下，上的 属性应在有效负载中使用类型说明符：</span><span class="sxs-lookup"><span data-stu-id="2312f-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="2312f-150">对于 `String` 类型属性，如果值包含非 ASCII 字符。</span><span class="sxs-lookup"><span data-stu-id="2312f-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="2312f-151">对于所有集合类型。</span><span class="sxs-lookup"><span data-stu-id="2312f-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="2312f-152">当包含 类型的 属性 `Collection(DateTime)` 时，必须使用类型说明器 `Collection(DateTimeOffset)` 。</span><span class="sxs-lookup"><span data-stu-id="2312f-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="2312f-153">响应</span><span class="sxs-lookup"><span data-stu-id="2312f-153">Response</span></span>

<span data-ttu-id="2312f-154">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2312f-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2312f-155">示例</span><span class="sxs-lookup"><span data-stu-id="2312f-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="2312f-156">示例：创建自定义项</span><span class="sxs-lookup"><span data-stu-id="2312f-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="2312f-157">请求</span><span class="sxs-lookup"><span data-stu-id="2312f-157">Request</span></span>

<span data-ttu-id="2312f-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2312f-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2312f-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="2312f-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
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
# <a name="c"></a>[<span data-ttu-id="2312f-160">C#</span><span class="sxs-lookup"><span data-stu-id="2312f-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2312f-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2312f-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2312f-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2312f-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="2312f-163">响应</span><span class="sxs-lookup"><span data-stu-id="2312f-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2312f-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2312f-164">The following is an example of the response.</span></span>

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
