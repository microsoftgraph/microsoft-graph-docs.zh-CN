---
title: 更新 externalitem
description: 更新 externalitem 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ff3237204310365eb8945a739bd423668494f786
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421996"
---
# <a name="update-externalitem"></a><span data-ttu-id="ac770-103">更新 externalitem</span><span class="sxs-lookup"><span data-stu-id="ac770-103">Update externalitem</span></span>

<span data-ttu-id="ac770-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ac770-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac770-105">更新[externalitem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="ac770-105">Update the properties of an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="ac770-106">权限</span><span class="sxs-lookup"><span data-stu-id="ac770-106">Permissions</span></span>

<span data-ttu-id="ac770-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac770-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac770-109">Permission type</span></span>                        | <span data-ttu-id="ac770-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac770-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ac770-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac770-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac770-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac770-112">Not supported.</span></span> |
| <span data-ttu-id="ac770-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac770-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac770-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac770-114">Not supported.</span></span> |
| <span data-ttu-id="ac770-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac770-115">Application</span></span>                            | <span data-ttu-id="ac770-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac770-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac770-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac770-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="ac770-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="ac770-118">Path parameters</span></span>

| <span data-ttu-id="ac770-119">参数</span><span class="sxs-lookup"><span data-stu-id="ac770-119">Parameter</span></span>     | <span data-ttu-id="ac770-120">类型</span><span class="sxs-lookup"><span data-stu-id="ac770-120">Type</span></span>   | <span data-ttu-id="ac770-121">说明</span><span class="sxs-lookup"><span data-stu-id="ac770-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="ac770-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="ac770-122">connection-id</span></span> | <span data-ttu-id="ac770-123">string</span><span class="sxs-lookup"><span data-stu-id="ac770-123">string</span></span> | <span data-ttu-id="ac770-124">包含`id` [externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="ac770-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="ac770-125">item-id</span><span class="sxs-lookup"><span data-stu-id="ac770-125">item-id</span></span>       | <span data-ttu-id="ac770-126">string</span><span class="sxs-lookup"><span data-stu-id="ac770-126">string</span></span> | <span data-ttu-id="ac770-127">开发人员提供`id`的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)属性。</span><span class="sxs-lookup"><span data-stu-id="ac770-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ac770-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac770-128">Request headers</span></span>

| <span data-ttu-id="ac770-129">名称</span><span class="sxs-lookup"><span data-stu-id="ac770-129">Name</span></span>          | <span data-ttu-id="ac770-130">说明</span><span class="sxs-lookup"><span data-stu-id="ac770-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="ac770-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac770-131">Authorization</span></span> | <span data-ttu-id="ac770-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac770-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ac770-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac770-134">Content-Type</span></span>  | <span data-ttu-id="ac770-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ac770-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac770-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac770-137">Request body</span></span>

<span data-ttu-id="ac770-138">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ac770-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ac770-139">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ac770-139">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ac770-140">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ac770-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="ac770-141">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="ac770-141">The following properties can be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="ac770-142">在预览过程中， `acl`可以通过修补程序来更新属性。</span><span class="sxs-lookup"><span data-stu-id="ac770-142">During the preview only the `acl` property can be updated via PATCH.</span></span> <span data-ttu-id="ac770-143">若要更新其他属性，请使用[PUT 将现有项改写为新项](externalconnection-put-items.md)。</span><span class="sxs-lookup"><span data-stu-id="ac770-143">In order to update other properties, use a [PUT to overwrite the existing item with a new item](externalconnection-put-items.md).</span></span>

### <a name="externalitem-properties"></a><span data-ttu-id="ac770-144">externalItem 属性</span><span class="sxs-lookup"><span data-stu-id="ac770-144">externalItem properties</span></span>

| <span data-ttu-id="ac770-145">属性</span><span class="sxs-lookup"><span data-stu-id="ac770-145">Property</span></span> | <span data-ttu-id="ac770-146">类型</span><span class="sxs-lookup"><span data-stu-id="ac770-146">Type</span></span>                                  | <span data-ttu-id="ac770-147">说明</span><span class="sxs-lookup"><span data-stu-id="ac770-147">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="ac770-148">acl</span><span class="sxs-lookup"><span data-stu-id="ac770-148">acl</span></span>      | <span data-ttu-id="ac770-149">[acl](../resources/acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac770-149">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="ac770-150">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="ac770-150">An array of access control entries.</span></span> <span data-ttu-id="ac770-151">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="ac770-151">Each entry specifies the access granted to a user or group.</span></span> |

### <a name="externalfile-properties"></a><span data-ttu-id="ac770-152">externalFile 属性</span><span class="sxs-lookup"><span data-stu-id="ac770-152">externalFile properties</span></span>

| <span data-ttu-id="ac770-153">属性</span><span class="sxs-lookup"><span data-stu-id="ac770-153">Property</span></span> | <span data-ttu-id="ac770-154">类型</span><span class="sxs-lookup"><span data-stu-id="ac770-154">Type</span></span>                                  | <span data-ttu-id="ac770-155">说明</span><span class="sxs-lookup"><span data-stu-id="ac770-155">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="ac770-156">acl</span><span class="sxs-lookup"><span data-stu-id="ac770-156">acl</span></span>      | <span data-ttu-id="ac770-157">[acl](../resources/acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac770-157">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="ac770-158">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="ac770-158">An array of access control entries.</span></span> <span data-ttu-id="ac770-159">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="ac770-159">Each entry specifies the access granted to a user or group.</span></span> |

## <a name="response"></a><span data-ttu-id="ac770-160">响应</span><span class="sxs-lookup"><span data-stu-id="ac770-160">Response</span></span>

<span data-ttu-id="ac770-161">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ac770-161">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac770-162">示例</span><span class="sxs-lookup"><span data-stu-id="ac770-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac770-163">请求</span><span class="sxs-lookup"><span data-stu-id="ac770-163">Request</span></span>

<span data-ttu-id="ac770-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac770-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac770-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac770-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac770-166">C#</span><span class="sxs-lookup"><span data-stu-id="ac770-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac770-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac770-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac770-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac770-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="ac770-169">响应</span><span class="sxs-lookup"><span data-stu-id="ac770-169">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="ac770-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac770-170">The following is an example of the response.</span></span>

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
  "content": "Textual content of the file"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
