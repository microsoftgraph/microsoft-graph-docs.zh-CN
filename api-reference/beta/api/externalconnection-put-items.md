---
title: 创建 externalItem
description: 创建新的 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 13c794fc7d03fa607bc61d57d731bdf2d3d04f71
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994547"
---
# <a name="create-externalitem"></a><span data-ttu-id="f7b9d-103">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="f7b9d-103">Create externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b9d-104">创建新的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-104">Create a new [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

<span data-ttu-id="f7b9d-105">此 API 可用于创建自定义项或文件。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-105">This API can be used to create a custom item or a file.</span></span> <span data-ttu-id="f7b9d-106">通过在 JSON 正文中包含`@odata.type`属性来指定要创建的类型。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-106">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="f7b9d-107">包含的[externalConnection](../resources/externalconnection.md)必须具有相应类型的已注册[架构](../resources/schema.md)。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-107">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b9d-108">权限</span><span class="sxs-lookup"><span data-stu-id="f7b9d-108">Permissions</span></span>

<span data-ttu-id="f7b9d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7b9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7b9d-111">Permission type</span></span>                        | <span data-ttu-id="f7b9d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7b9d-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7b9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b9d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7b9d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-114">Not supported.</span></span> |
| <span data-ttu-id="f7b9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-116">Not supported.</span></span> |
| <span data-ttu-id="f7b9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7b9d-117">Application</span></span>                            | <span data-ttu-id="f7b9d-118">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7b9d-118">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7b9d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="f7b9d-120">路径参数</span><span class="sxs-lookup"><span data-stu-id="f7b9d-120">Path parameters</span></span>

| <span data-ttu-id="f7b9d-121">参数</span><span class="sxs-lookup"><span data-stu-id="f7b9d-121">Parameter</span></span>     | <span data-ttu-id="f7b9d-122">类型</span><span class="sxs-lookup"><span data-stu-id="f7b9d-122">Type</span></span>   | <span data-ttu-id="f7b9d-123">说明</span><span class="sxs-lookup"><span data-stu-id="f7b9d-123">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="f7b9d-124">connection-id</span><span class="sxs-lookup"><span data-stu-id="f7b9d-124">connection-id</span></span> | <span data-ttu-id="f7b9d-125">string</span><span class="sxs-lookup"><span data-stu-id="f7b9d-125">string</span></span> | <span data-ttu-id="f7b9d-126">包含`id` [externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="f7b9d-126">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="f7b9d-127">item-id</span><span class="sxs-lookup"><span data-stu-id="f7b9d-127">item-id</span></span>       | <span data-ttu-id="f7b9d-128">string</span><span class="sxs-lookup"><span data-stu-id="f7b9d-128">string</span></span> | <span data-ttu-id="f7b9d-129">开发人员提供`id`的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)属性。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-129">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> <span data-ttu-id="f7b9d-130">如果不存在具有此`id`项的项目，则会创建一个新项目。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-130">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="f7b9d-131">如果某个项目已经存在`id`，则会被在正文中发送的对象覆盖。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-131">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f7b9d-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7b9d-132">Request headers</span></span>

| <span data-ttu-id="f7b9d-133">名称</span><span class="sxs-lookup"><span data-stu-id="f7b9d-133">Name</span></span>          | <span data-ttu-id="f7b9d-134">说明</span><span class="sxs-lookup"><span data-stu-id="f7b9d-134">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="f7b9d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7b9d-135">Authorization</span></span> | <span data-ttu-id="f7b9d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f7b9d-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7b9d-138">Content-Type</span></span>  | <span data-ttu-id="f7b9d-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f7b9d-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7b9d-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7b9d-141">Request body</span></span>

<span data-ttu-id="f7b9d-142">在请求正文中，提供[externalItem](../resources/externalitem.md)或[EXTERNALFILE](../resources/externalfile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-142">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object.</span></span> <span data-ttu-id="f7b9d-143">有效负载限制为 4 MB。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-143">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="f7b9d-144">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="f7b9d-144">Creating an externalItem</span></span>

<span data-ttu-id="f7b9d-145">在创建时`externalItem`，需要以下字段： `@odata.type`、 `acl`和。 `properties`</span><span class="sxs-lookup"><span data-stu-id="f7b9d-145">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="f7b9d-146">该`properties`对象必须至少包含一个属性。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-146">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="f7b9d-147">所有`DateTime`类型属性都必须采用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-147">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="f7b9d-148">中的属性`externalItem`应在以下方案中使用有效负载中的类型说明符：</span><span class="sxs-lookup"><span data-stu-id="f7b9d-148">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="f7b9d-149">对于`String` type 属性，如果该值包含非 ASCII 字符。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-149">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="f7b9d-150">适用于所有集合类型。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-150">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="f7b9d-151">如果包含类型`Collection(DateTime)`的属性，则必须使用类型说明符`Collection(DateTimeOffset)`。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-151">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

### <a name="creating-an-externalfile"></a><span data-ttu-id="f7b9d-152">创建 externalFile</span><span class="sxs-lookup"><span data-stu-id="f7b9d-152">Creating an externalFile</span></span>

<span data-ttu-id="f7b9d-153">在创建时`externalFile`，需要以下字段`@odata.type`：、 `acl` `name`、和。 `url`</span><span class="sxs-lookup"><span data-stu-id="f7b9d-153">When creating an `externalFile`, the following fields are required: `@odata.type`, `acl`, `name`, and `url`.</span></span>

## <a name="response"></a><span data-ttu-id="f7b9d-154">响应</span><span class="sxs-lookup"><span data-stu-id="f7b9d-154">Response</span></span>

<span data-ttu-id="f7b9d-155">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-155">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f7b9d-156">示例</span><span class="sxs-lookup"><span data-stu-id="f7b9d-156">Examples</span></span>

### <a name="example-1-create-a-custom-item"></a><span data-ttu-id="f7b9d-157">示例1：创建自定义项</span><span class="sxs-lookup"><span data-stu-id="f7b9d-157">Example 1: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="f7b9d-158">请求</span><span class="sxs-lookup"><span data-stu-id="f7b9d-158">Request</span></span>

<span data-ttu-id="f7b9d-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-159">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7b9d-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b9d-160">HTTP</span></span>](#tab/http)
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
      "identitySource": "Azure Active Directory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": "Textual content of the file"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7b9d-161">C#</span><span class="sxs-lookup"><span data-stu-id="f7b9d-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7b9d-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7b9d-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7b9d-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7b9d-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="f7b9d-164">响应</span><span class="sxs-lookup"><span data-stu-id="f7b9d-164">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f7b9d-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

### <a name="example-2-create-a-file"></a><span data-ttu-id="f7b9d-166">示例2：创建文件</span><span class="sxs-lookup"><span data-stu-id="f7b9d-166">Example 2: Create a file</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="f7b9d-167">请求</span><span class="sxs-lookup"><span data-stu-id="f7b9d-167">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f7b9d-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-168">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7b9d-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b9d-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalfile_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosofiles/items/myFile01
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalFile",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ],
  "createdDateTime": "2019-01-31T03:44:19.0354159Z",
  "modifiedDateTime": "2019-01-31T03:44:19.0354159Z",
  "createdBy": "Pradeep Gupta",
  "lastModifiedBy": "Adele Vance",
  "title": "Enterprise Search Graph Ingestion API",
  "url": "file://filesrv02.corp.contoso.com/data/project/Enterprise Search.docx",
  "name": "Enterprise Search.docx",
  "extension": "docx",
  "size": 8676776,
  "content": "The quick brown fox jumps over the lazy dog."
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7b9d-170">C#</span><span class="sxs-lookup"><span data-stu-id="f7b9d-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalfile-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7b9d-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7b9d-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalfile-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7b9d-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7b9d-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalfile-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="f7b9d-173">响应</span><span class="sxs-lookup"><span data-stu-id="f7b9d-173">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f7b9d-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7b9d-174">The following is an example of the response.</span></span>

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
