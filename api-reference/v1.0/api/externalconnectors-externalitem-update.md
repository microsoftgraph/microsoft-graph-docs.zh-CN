---
title: 更新 externalItem
description: 更新 externalItem 对象的属性。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 10c59c40dd5ae889469b00b708b852326a2fd0e8
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467284"
---
# <a name="update-externalitem"></a><span data-ttu-id="9e798-103">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="9e798-103">Update externalItem</span></span>
<span data-ttu-id="9e798-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="9e798-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="9e798-105">更新 [externalItem 对象](../resources/externalconnectors-externalitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9e798-105">Update the properties of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e798-106">权限</span><span class="sxs-lookup"><span data-stu-id="9e798-106">Permissions</span></span>
<span data-ttu-id="9e798-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e798-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e798-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e798-109">Permission type</span></span>|<span data-ttu-id="9e798-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e798-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e798-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e798-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e798-112">不适用</span><span class="sxs-lookup"><span data-stu-id="9e798-112">Not applicable</span></span>|
|<span data-ttu-id="9e798-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e798-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e798-114">不适用</span><span class="sxs-lookup"><span data-stu-id="9e798-114">Not applicable</span></span>|
|<span data-ttu-id="9e798-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e798-115">Application</span></span>| <span data-ttu-id="9e798-116">ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e798-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e798-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e798-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="9e798-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="9e798-118">Path parameters</span></span>

| <span data-ttu-id="9e798-119">参数</span><span class="sxs-lookup"><span data-stu-id="9e798-119">Parameter</span></span>     | <span data-ttu-id="9e798-120">类型</span><span class="sxs-lookup"><span data-stu-id="9e798-120">Type</span></span>   | <span data-ttu-id="9e798-121">说明</span><span class="sxs-lookup"><span data-stu-id="9e798-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="9e798-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="9e798-122">connection-id</span></span> | <span data-ttu-id="9e798-123">string</span><span class="sxs-lookup"><span data-stu-id="9e798-123">string</span></span> | <span data-ttu-id="9e798-124">`id`包含[externalConnection 的 属性](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="9e798-124">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="9e798-125">item-id</span><span class="sxs-lookup"><span data-stu-id="9e798-125">item-id</span></span>       | <span data-ttu-id="9e798-126">string</span><span class="sxs-lookup"><span data-stu-id="9e798-126">string</span></span> | <span data-ttu-id="9e798-127">由开发人员提供的 `id` [externalItem 属性](../resources/externalconnectors-externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="9e798-127">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9e798-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e798-128">Request headers</span></span>

| <span data-ttu-id="9e798-129">名称</span><span class="sxs-lookup"><span data-stu-id="9e798-129">Name</span></span>          | <span data-ttu-id="9e798-130">说明</span><span class="sxs-lookup"><span data-stu-id="9e798-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="9e798-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e798-131">Authorization</span></span> | <span data-ttu-id="9e798-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e798-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9e798-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e798-134">Content-Type</span></span>  | <span data-ttu-id="9e798-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9e798-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e798-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e798-137">Request body</span></span>

<span data-ttu-id="9e798-138">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9e798-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9e798-139">现有 (不包括请求正文) 对象对象中的属性将保留其以前的值或根据其他属性值的更改 `properties` 重新计算。</span><span class="sxs-lookup"><span data-stu-id="9e798-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9e798-140">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9e798-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="9e798-141">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="9e798-141">The following properties can be updated.</span></span>

| <span data-ttu-id="9e798-142">属性</span><span class="sxs-lookup"><span data-stu-id="9e798-142">Property</span></span>   | <span data-ttu-id="9e798-143">类型</span><span class="sxs-lookup"><span data-stu-id="9e798-143">Type</span></span>                                  | <span data-ttu-id="9e798-144">说明</span><span class="sxs-lookup"><span data-stu-id="9e798-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="9e798-145">acl</span><span class="sxs-lookup"><span data-stu-id="9e798-145">acl</span></span>        | <span data-ttu-id="9e798-146">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e798-146">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) collection</span></span> | <span data-ttu-id="9e798-147">访问控制项数组。</span><span class="sxs-lookup"><span data-stu-id="9e798-147">An array of access control entries.</span></span> <span data-ttu-id="9e798-148">每个条目指定授予用户或组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="9e798-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="9e798-149">content</span><span class="sxs-lookup"><span data-stu-id="9e798-149">content</span></span>    | [<span data-ttu-id="9e798-150">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="9e798-150">microsoft.graph.externalConnectors.externalItemContent</span></span>](../resources/externalconnectors-externalitemcontent.md) | <span data-ttu-id="9e798-151">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e798-151">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="9e798-152">此属性中的文本已编制全文索引。</span><span class="sxs-lookup"><span data-stu-id="9e798-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="9e798-153">properties</span><span class="sxs-lookup"><span data-stu-id="9e798-153">properties</span></span> | <span data-ttu-id="9e798-154">Object</span><span class="sxs-lookup"><span data-stu-id="9e798-154">Object</span></span>                              | <span data-ttu-id="9e798-155">具有项目属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="9e798-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="9e798-156">属性必须符合为[externalConnection](../resources/externalconnectors-externalconnection.md)定义的架构。 [](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="9e798-156">The properties MUST conform to the [schema](../resources/externalconnectors-schema.md) defined for the [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="9e798-157">更新 acl 集合</span><span class="sxs-lookup"><span data-stu-id="9e798-157">Updating the acl collection</span></span>

<span data-ttu-id="9e798-158">如果属性包含在更新请求中，则现有 ACL 集合将被请求中包含的集合 `acl` 覆盖。</span><span class="sxs-lookup"><span data-stu-id="9e798-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="9e798-159">更新 properties 对象</span><span class="sxs-lookup"><span data-stu-id="9e798-159">Updating the properties object</span></span>

<span data-ttu-id="9e798-160">如果属性包含在更新请求中，则现有属性包将被请求 `properties` 中包含的值覆盖。</span><span class="sxs-lookup"><span data-stu-id="9e798-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="9e798-161">响应</span><span class="sxs-lookup"><span data-stu-id="9e798-161">Response</span></span>

<span data-ttu-id="9e798-162">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [externalItem](../resources/externalconnectors-externalitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e798-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalconnectors-externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e798-163">示例</span><span class="sxs-lookup"><span data-stu-id="9e798-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e798-164">请求</span><span class="sxs-lookup"><span data-stu-id="9e798-164">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_externalitem",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
Content-Type: application/json
Content-length: 360

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="9e798-165">响应</span><span class="sxs-lookup"><span data-stu-id="9e798-165">Response</span></span>
<span data-ttu-id="9e798-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9e798-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent",
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