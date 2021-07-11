---
title: 更新 externalitem
description: 更新 externalitem 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c862a6139f4f24a9207e7387913ec0fc5b04e8e6
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366786"
---
# <a name="update-externalitem"></a><span data-ttu-id="c8ffc-103">更新 externalitem</span><span class="sxs-lookup"><span data-stu-id="c8ffc-103">Update externalitem</span></span>

<span data-ttu-id="c8ffc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8ffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8ffc-105">更新 [externalitem 的属性](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-105">Update the properties of an [externalitem](../resources/externalitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8ffc-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c8ffc-106">Permissions</span></span>

<span data-ttu-id="c8ffc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8ffc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8ffc-109">Permission type</span></span>                        | <span data-ttu-id="c8ffc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8ffc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8ffc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8ffc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8ffc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-112">Not supported.</span></span> |
| <span data-ttu-id="c8ffc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8ffc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8ffc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-114">Not supported.</span></span> |
| <span data-ttu-id="c8ffc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8ffc-115">Application</span></span>                            | <span data-ttu-id="c8ffc-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ffc-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8ffc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8ffc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="c8ffc-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="c8ffc-118">Path parameters</span></span>

| <span data-ttu-id="c8ffc-119">参数</span><span class="sxs-lookup"><span data-stu-id="c8ffc-119">Parameter</span></span>     | <span data-ttu-id="c8ffc-120">类型</span><span class="sxs-lookup"><span data-stu-id="c8ffc-120">Type</span></span>   | <span data-ttu-id="c8ffc-121">说明</span><span class="sxs-lookup"><span data-stu-id="c8ffc-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="c8ffc-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="c8ffc-122">connection-id</span></span> | <span data-ttu-id="c8ffc-123">string</span><span class="sxs-lookup"><span data-stu-id="c8ffc-123">string</span></span> | <span data-ttu-id="c8ffc-124">`id`包含[externalConnection 的 属性](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="c8ffc-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="c8ffc-125">item-id</span><span class="sxs-lookup"><span data-stu-id="c8ffc-125">item-id</span></span>       | <span data-ttu-id="c8ffc-126">string</span><span class="sxs-lookup"><span data-stu-id="c8ffc-126">string</span></span> | <span data-ttu-id="c8ffc-127">由开发人员提供的 `id` [externalItem 属性](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c8ffc-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8ffc-128">Request headers</span></span>

| <span data-ttu-id="c8ffc-129">名称</span><span class="sxs-lookup"><span data-stu-id="c8ffc-129">Name</span></span>          | <span data-ttu-id="c8ffc-130">说明</span><span class="sxs-lookup"><span data-stu-id="c8ffc-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="c8ffc-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8ffc-131">Authorization</span></span> | <span data-ttu-id="c8ffc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c8ffc-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8ffc-134">Content-Type</span></span>  | <span data-ttu-id="c8ffc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c8ffc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8ffc-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8ffc-137">Request body</span></span>

<span data-ttu-id="c8ffc-138">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c8ffc-139">现有 (不包括请求正文) 对象对象中的属性将保留其以前的值或根据其他属性值的更改 `properties` 重新计算。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c8ffc-140">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="c8ffc-141">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-141">The following properties can be updated.</span></span>

| <span data-ttu-id="c8ffc-142">属性</span><span class="sxs-lookup"><span data-stu-id="c8ffc-142">Property</span></span>   | <span data-ttu-id="c8ffc-143">类型</span><span class="sxs-lookup"><span data-stu-id="c8ffc-143">Type</span></span>                                  | <span data-ttu-id="c8ffc-144">说明</span><span class="sxs-lookup"><span data-stu-id="c8ffc-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="c8ffc-145">acl</span><span class="sxs-lookup"><span data-stu-id="c8ffc-145">acl</span></span>        | <span data-ttu-id="c8ffc-146">[acl](../resources/acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8ffc-146">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="c8ffc-147">访问控制项数组。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-147">An array of access control entries.</span></span> <span data-ttu-id="c8ffc-148">每个条目指定授予用户或组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="c8ffc-149">content</span><span class="sxs-lookup"><span data-stu-id="c8ffc-149">content</span></span>    | [<span data-ttu-id="c8ffc-150">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="c8ffc-150">externalItemContent</span></span>](../resources/externalitemcontent.md) | <span data-ttu-id="c8ffc-151">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-151">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="c8ffc-152">此属性中的文本已编制全文索引。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="c8ffc-153">properties</span><span class="sxs-lookup"><span data-stu-id="c8ffc-153">properties</span></span> | <span data-ttu-id="c8ffc-154">Object</span><span class="sxs-lookup"><span data-stu-id="c8ffc-154">Object</span></span>                                | <span data-ttu-id="c8ffc-155">具有项目属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="c8ffc-156">属性必须符合为[externalConnection](../resources/externalconnection.md)定义的架构。 [](../resources/schema.md)</span><span class="sxs-lookup"><span data-stu-id="c8ffc-156">The properties MUST conform to the [schema](../resources/schema.md) defined for the [externalConnection](../resources/externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="c8ffc-157">更新 acl 集合</span><span class="sxs-lookup"><span data-stu-id="c8ffc-157">Updating the acl collection</span></span>

<span data-ttu-id="c8ffc-158">如果属性包含在更新请求中，则现有 ACL 集合将被请求中包含的集合 `acl` 覆盖。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="c8ffc-159">更新 properties 对象</span><span class="sxs-lookup"><span data-stu-id="c8ffc-159">Updating the properties object</span></span>

<span data-ttu-id="c8ffc-160">如果属性包含在更新请求中，则现有属性包将被请求 `properties` 中包含的值覆盖。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="c8ffc-161">响应</span><span class="sxs-lookup"><span data-stu-id="c8ffc-161">Response</span></span>

<span data-ttu-id="c8ffc-162">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [externalItem](../resources/externalitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8ffc-163">示例</span><span class="sxs-lookup"><span data-stu-id="c8ffc-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8ffc-164">请求</span><span class="sxs-lookup"><span data-stu-id="c8ffc-164">Request</span></span>

<span data-ttu-id="c8ffc-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8ffc-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8ffc-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c8ffc-167">C#</span><span class="sxs-lookup"><span data-stu-id="c8ffc-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8ffc-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8ffc-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8ffc-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8ffc-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8ffc-170">Java</span><span class="sxs-lookup"><span data-stu-id="c8ffc-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="c8ffc-171">响应</span><span class="sxs-lookup"><span data-stu-id="c8ffc-171">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="c8ffc-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c8ffc-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_externalitem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->


