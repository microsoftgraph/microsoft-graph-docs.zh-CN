---
title: 更新 externalitem
description: 更新 externalitem 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 05eef675ccb6b79e3919fae9a50e90b2d9a31326
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747195"
---
# <a name="update-externalitem"></a><span data-ttu-id="e2112-103">更新 externalitem</span><span class="sxs-lookup"><span data-stu-id="e2112-103">Update externalitem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2112-104">更新[externalitem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="e2112-104">Update the properties of an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="e2112-105">权限</span><span class="sxs-lookup"><span data-stu-id="e2112-105">Permissions</span></span>

<span data-ttu-id="e2112-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2112-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2112-108">Permission type</span></span>                        | <span data-ttu-id="e2112-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2112-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2112-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2112-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2112-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2112-111">Not supported.</span></span> |
| <span data-ttu-id="e2112-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2112-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2112-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2112-113">Not supported.</span></span> |
| <span data-ttu-id="e2112-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2112-114">Application</span></span>                            | <span data-ttu-id="e2112-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2112-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2112-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2112-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="e2112-117">路径参数</span><span class="sxs-lookup"><span data-stu-id="e2112-117">Path parameters</span></span>

| <span data-ttu-id="e2112-118">参数</span><span class="sxs-lookup"><span data-stu-id="e2112-118">Parameter</span></span>     | <span data-ttu-id="e2112-119">类型</span><span class="sxs-lookup"><span data-stu-id="e2112-119">Type</span></span>   | <span data-ttu-id="e2112-120">说明</span><span class="sxs-lookup"><span data-stu-id="e2112-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="e2112-121">connection-id</span><span class="sxs-lookup"><span data-stu-id="e2112-121">connection-id</span></span> | <span data-ttu-id="e2112-122">字符串</span><span class="sxs-lookup"><span data-stu-id="e2112-122">string</span></span> | <span data-ttu-id="e2112-123">包含`id` [externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="e2112-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="e2112-124">item-id</span><span class="sxs-lookup"><span data-stu-id="e2112-124">item-id</span></span>       | <span data-ttu-id="e2112-125">字符串</span><span class="sxs-lookup"><span data-stu-id="e2112-125">string</span></span> | <span data-ttu-id="e2112-126">开发人员提供`id`的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)属性。</span><span class="sxs-lookup"><span data-stu-id="e2112-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e2112-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2112-127">Request headers</span></span>

| <span data-ttu-id="e2112-128">名称</span><span class="sxs-lookup"><span data-stu-id="e2112-128">Name</span></span>          | <span data-ttu-id="e2112-129">说明</span><span class="sxs-lookup"><span data-stu-id="e2112-129">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="e2112-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2112-130">Authorization</span></span> | <span data-ttu-id="e2112-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2112-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e2112-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2112-133">Content-Type</span></span>  | <span data-ttu-id="e2112-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e2112-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2112-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2112-136">Request body</span></span>

<span data-ttu-id="e2112-137">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e2112-137">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e2112-138">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e2112-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e2112-139">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e2112-139">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="e2112-140">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="e2112-140">The following properties can be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="e2112-141">在预览过程中， `acl`可以通过修补程序来更新属性。</span><span class="sxs-lookup"><span data-stu-id="e2112-141">During the preview only the `acl` property can be updated via PATCH.</span></span> <span data-ttu-id="e2112-142">若要更新其他属性，请使用[PUT 将现有项改写为新项](externalconnection-put-items.md)。</span><span class="sxs-lookup"><span data-stu-id="e2112-142">In order to update other properties, use a [PUT to overwrite the existing item with a new item](externalconnection-put-items.md).</span></span>

### <a name="externalitem-properties"></a><span data-ttu-id="e2112-143">externalItem 属性</span><span class="sxs-lookup"><span data-stu-id="e2112-143">externalItem properties</span></span>

| <span data-ttu-id="e2112-144">属性</span><span class="sxs-lookup"><span data-stu-id="e2112-144">Property</span></span> | <span data-ttu-id="e2112-145">类型</span><span class="sxs-lookup"><span data-stu-id="e2112-145">Type</span></span>                                  | <span data-ttu-id="e2112-146">说明</span><span class="sxs-lookup"><span data-stu-id="e2112-146">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="e2112-147">acl</span><span class="sxs-lookup"><span data-stu-id="e2112-147">acl</span></span>      | <span data-ttu-id="e2112-148">[acl](../resources/acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2112-148">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="e2112-149">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="e2112-149">An array of access control entries.</span></span> <span data-ttu-id="e2112-150">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="e2112-150">Each entry specifies the access granted to a user or group.</span></span> |

### <a name="externalfile-properties"></a><span data-ttu-id="e2112-151">externalFile 属性</span><span class="sxs-lookup"><span data-stu-id="e2112-151">externalFile properties</span></span>

| <span data-ttu-id="e2112-152">属性</span><span class="sxs-lookup"><span data-stu-id="e2112-152">Property</span></span> | <span data-ttu-id="e2112-153">类型</span><span class="sxs-lookup"><span data-stu-id="e2112-153">Type</span></span>                                  | <span data-ttu-id="e2112-154">说明</span><span class="sxs-lookup"><span data-stu-id="e2112-154">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="e2112-155">acl</span><span class="sxs-lookup"><span data-stu-id="e2112-155">acl</span></span>      | <span data-ttu-id="e2112-156">[acl](../resources/acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2112-156">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="e2112-157">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="e2112-157">An array of access control entries.</span></span> <span data-ttu-id="e2112-158">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="e2112-158">Each entry specifies the access granted to a user or group.</span></span> |

## <a name="response"></a><span data-ttu-id="e2112-159">响应</span><span class="sxs-lookup"><span data-stu-id="e2112-159">Response</span></span>

<span data-ttu-id="e2112-160">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2112-160">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2112-161">示例</span><span class="sxs-lookup"><span data-stu-id="e2112-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2112-162">请求</span><span class="sxs-lookup"><span data-stu-id="e2112-162">Request</span></span>

<span data-ttu-id="e2112-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2112-163">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2112-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2112-164">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2112-165">C#</span><span class="sxs-lookup"><span data-stu-id="e2112-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2112-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2112-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2112-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2112-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="e2112-168">响应</span><span class="sxs-lookup"><span data-stu-id="e2112-168">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="e2112-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e2112-169">The following is an example of the response.</span></span>

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
