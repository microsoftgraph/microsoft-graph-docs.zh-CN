---
title: 更新 externalitem
description: 更新 externalitem 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: de4b983592978ca05b2e2db8fe1eccd0697147fb
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718617"
---
# <a name="update-externalitem"></a><span data-ttu-id="cc0f8-103">更新 externalitem</span><span class="sxs-lookup"><span data-stu-id="cc0f8-103">Update externalitem</span></span>

<span data-ttu-id="cc0f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc0f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc0f8-105">更新[externalitem](../resources/externalitem.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-105">Update the properties of an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="cc0f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="cc0f8-106">Permissions</span></span>

<span data-ttu-id="cc0f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc0f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc0f8-109">Permission type</span></span>                        | <span data-ttu-id="cc0f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc0f8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc0f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc0f8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc0f8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-112">Not supported.</span></span> |
| <span data-ttu-id="cc0f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc0f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc0f8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-114">Not supported.</span></span> |
| <span data-ttu-id="cc0f8-115">Application</span><span class="sxs-lookup"><span data-stu-id="cc0f8-115">Application</span></span>                            | <span data-ttu-id="cc0f8-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc0f8-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc0f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc0f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="cc0f8-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="cc0f8-118">Path parameters</span></span>

| <span data-ttu-id="cc0f8-119">参数</span><span class="sxs-lookup"><span data-stu-id="cc0f8-119">Parameter</span></span>     | <span data-ttu-id="cc0f8-120">类型</span><span class="sxs-lookup"><span data-stu-id="cc0f8-120">Type</span></span>   | <span data-ttu-id="cc0f8-121">说明</span><span class="sxs-lookup"><span data-stu-id="cc0f8-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="cc0f8-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="cc0f8-122">connection-id</span></span> | <span data-ttu-id="cc0f8-123">string</span><span class="sxs-lookup"><span data-stu-id="cc0f8-123">string</span></span> | <span data-ttu-id="cc0f8-124">包含`id` [externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="cc0f8-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="cc0f8-125">item-id</span><span class="sxs-lookup"><span data-stu-id="cc0f8-125">item-id</span></span>       | <span data-ttu-id="cc0f8-126">string</span><span class="sxs-lookup"><span data-stu-id="cc0f8-126">string</span></span> | <span data-ttu-id="cc0f8-127">ExternalItem 的开发人员`id`提供的属性[externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cc0f8-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc0f8-128">Request headers</span></span>

| <span data-ttu-id="cc0f8-129">名称</span><span class="sxs-lookup"><span data-stu-id="cc0f8-129">Name</span></span>          | <span data-ttu-id="cc0f8-130">说明</span><span class="sxs-lookup"><span data-stu-id="cc0f8-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="cc0f8-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc0f8-131">Authorization</span></span> | <span data-ttu-id="cc0f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="cc0f8-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc0f8-134">Content-Type</span></span>  | <span data-ttu-id="cc0f8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cc0f8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc0f8-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc0f8-137">Request body</span></span>

<span data-ttu-id="cc0f8-138">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cc0f8-139">未包含在请求正文中的`properties`现有属性（对象内的属性除外）将保留其以前的值，或根据对其他属性值的更改重新计算这些属性。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cc0f8-140">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="cc0f8-141">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-141">The following properties can be updated.</span></span>

| <span data-ttu-id="cc0f8-142">属性</span><span class="sxs-lookup"><span data-stu-id="cc0f8-142">Property</span></span>   | <span data-ttu-id="cc0f8-143">类型</span><span class="sxs-lookup"><span data-stu-id="cc0f8-143">Type</span></span>                                  | <span data-ttu-id="cc0f8-144">说明</span><span class="sxs-lookup"><span data-stu-id="cc0f8-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="cc0f8-145">acl</span><span class="sxs-lookup"><span data-stu-id="cc0f8-145">acl</span></span>        | <span data-ttu-id="cc0f8-146">[acl](../resources/acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc0f8-146">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="cc0f8-147">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-147">An array of access control entries.</span></span> <span data-ttu-id="cc0f8-148">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="cc0f8-149">content</span><span class="sxs-lookup"><span data-stu-id="cc0f8-149">content</span></span>    | [<span data-ttu-id="cc0f8-150">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="cc0f8-150">externalItemContent</span></span>](../resources/externalitemcontent.md) | <span data-ttu-id="cc0f8-151">项目内容的纯文本或 HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-151">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="cc0f8-152">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="cc0f8-153">properties</span><span class="sxs-lookup"><span data-stu-id="cc0f8-153">properties</span></span> | <span data-ttu-id="cc0f8-154">对象</span><span class="sxs-lookup"><span data-stu-id="cc0f8-154">Object</span></span>                                | <span data-ttu-id="cc0f8-155">包含项属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="cc0f8-156">属性必须符合为[externalConnection](../resources/externalconnection.md)定义的[架构](../resources/schema.md)。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-156">The properties MUST conform to the [schema](../resources/schema.md) defined for the [externalConnection](../resources/externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="cc0f8-157">更新 acl 集合</span><span class="sxs-lookup"><span data-stu-id="cc0f8-157">Updating the acl collection</span></span>

<span data-ttu-id="cc0f8-158">如果该`acl`属性包含在更新请求中，则将使用请求中包含的集合覆盖现有的 ACL 集合。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="cc0f8-159">更新 properties 对象</span><span class="sxs-lookup"><span data-stu-id="cc0f8-159">Updating the properties object</span></span>

<span data-ttu-id="cc0f8-160">如果该`properties`属性包含在更新请求中，则现有属性包将被请求中包含的值覆盖。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="cc0f8-161">响应</span><span class="sxs-lookup"><span data-stu-id="cc0f8-161">Response</span></span>

<span data-ttu-id="cc0f8-162">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[externalItem](../resources/externalitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc0f8-163">示例</span><span class="sxs-lookup"><span data-stu-id="cc0f8-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc0f8-164">请求</span><span class="sxs-lookup"><span data-stu-id="cc0f8-164">Request</span></span>

<span data-ttu-id="cc0f8-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc0f8-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc0f8-166">HTTP</span></span>](#tab/http)
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
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="cc0f8-167">C#</span><span class="sxs-lookup"><span data-stu-id="cc0f8-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc0f8-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc0f8-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc0f8-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc0f8-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="cc0f8-170">响应</span><span class="sxs-lookup"><span data-stu-id="cc0f8-170">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="cc0f8-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc0f8-171">The following is an example of the response.</span></span>

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
      "identitySource": "Azure Active Directory"
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
