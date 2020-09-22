---
title: 更新 ipnamedlocation
description: 更新 ipNamedLocation 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1e9ff22fb86400214f283cb4e09fb0097f7843b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980062"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="d3dc9-103">更新 ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="d3dc9-103">Update ipNamedlocation</span></span>

<span data-ttu-id="d3dc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3dc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3dc9-105">更新 [ipNamedLocation](../resources/ipNamedLocation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-105">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3dc9-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3dc9-106">Permissions</span></span>

<span data-ttu-id="d3dc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3dc9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3dc9-109">Permission type</span></span>                        | <span data-ttu-id="d3dc9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3dc9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3dc9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3dc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3dc9-112">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d3dc9-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="d3dc9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3dc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3dc9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-114">Not supported.</span></span> |
| <span data-ttu-id="d3dc9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3dc9-115">Application</span></span>                            | <span data-ttu-id="d3dc9-116">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d3dc9-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3dc9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3dc9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d3dc9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3dc9-118">Request headers</span></span>

| <span data-ttu-id="d3dc9-119">名称</span><span class="sxs-lookup"><span data-stu-id="d3dc9-119">Name</span></span>       | <span data-ttu-id="d3dc9-120">说明</span><span class="sxs-lookup"><span data-stu-id="d3dc9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d3dc9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3dc9-121">Authorization</span></span> | <span data-ttu-id="d3dc9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3dc9-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="d3dc9-124">Content-type</span></span> | <span data-ttu-id="d3dc9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3dc9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3dc9-127">Request body</span></span>

<span data-ttu-id="d3dc9-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d3dc9-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d3dc9-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d3dc9-131">属性</span><span class="sxs-lookup"><span data-stu-id="d3dc9-131">Property</span></span>     | <span data-ttu-id="d3dc9-132">类型</span><span class="sxs-lookup"><span data-stu-id="d3dc9-132">Type</span></span>        | <span data-ttu-id="d3dc9-133">说明</span><span class="sxs-lookup"><span data-stu-id="d3dc9-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d3dc9-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d3dc9-134">displayName</span></span>|<span data-ttu-id="d3dc9-135">String</span><span class="sxs-lookup"><span data-stu-id="d3dc9-135">String</span></span>|<span data-ttu-id="d3dc9-136">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-136">Human-readable name of the location.</span></span>|
|<span data-ttu-id="d3dc9-137">ipRanges</span><span class="sxs-lookup"><span data-stu-id="d3dc9-137">ipRanges</span></span>|<span data-ttu-id="d3dc9-138">[ipRange](../resources/iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3dc9-138">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="d3dc9-139">IPv4 CIDR 格式的 IP 地址范围列表 (1.2.3.4/32) 或来自 IETF RFC5962 的任何允许的 IPv6 格式。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-139">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="d3dc9-140">isTrusted</span><span class="sxs-lookup"><span data-stu-id="d3dc9-140">isTrusted</span></span>|<span data-ttu-id="d3dc9-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3dc9-141">Boolean</span></span>|<span data-ttu-id="d3dc9-142">`true`如果此位置是明确信任的，则该值为。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-142">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="d3dc9-143">响应</span><span class="sxs-lookup"><span data-stu-id="d3dc9-143">Response</span></span>

<span data-ttu-id="d3dc9-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3dc9-146">示例</span><span class="sxs-lookup"><span data-stu-id="d3dc9-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3dc9-147">请求</span><span class="sxs-lookup"><span data-stu-id="d3dc9-147">Request</span></span>

<span data-ttu-id="d3dc9-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3dc9-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3dc9-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted named location with only IPv4 address",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "6.5.4.3/18"
        }

    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="d3dc9-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3dc9-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d3dc9-151">C#</span><span class="sxs-lookup"><span data-stu-id="d3dc9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3dc9-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3dc9-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3dc9-153">响应</span><span class="sxs-lookup"><span data-stu-id="d3dc9-153">Response</span></span>

<span data-ttu-id="d3dc9-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-154">The following is an example of the response.</span></span>

> <span data-ttu-id="d3dc9-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d3dc9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ipnamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


