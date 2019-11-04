---
title: 更新 ipnamedlocation
description: 更新 ipNamedLocation 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2658baafbe4fadf164004f99f56b9288545c2b8c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938457"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="0d4c7-103">更新 ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="0d4c7-103">Update ipNamedlocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d4c7-104">更新[ipNamedLocation](../resources/ipNamedLocation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-104">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d4c7-105">权限</span><span class="sxs-lookup"><span data-stu-id="0d4c7-105">Permissions</span></span>

<span data-ttu-id="0d4c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d4c7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d4c7-108">Permission type</span></span>                        | <span data-ttu-id="0d4c7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d4c7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d4c7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d4c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d4c7-111">ConditionalAccess 和 Directory.accessasuser.all 的所有</span><span class="sxs-lookup"><span data-stu-id="0d4c7-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="0d4c7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d4c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d4c7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-113">Not supported.</span></span> |
| <span data-ttu-id="0d4c7-114">Application</span><span class="sxs-lookup"><span data-stu-id="0d4c7-114">Application</span></span>                            | <span data-ttu-id="0d4c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="0d4c7-116">此 API 需要多个权限。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-116">This API requires multiple permissions.</span></span> <span data-ttu-id="0d4c7-117">有关详细信息，请参阅[已知问题](/graph/known-issues#conditional-access-policies-and-named-locations)。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="0d4c7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d4c7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d4c7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d4c7-119">Request headers</span></span>

| <span data-ttu-id="0d4c7-120">名称</span><span class="sxs-lookup"><span data-stu-id="0d4c7-120">Name</span></span>       | <span data-ttu-id="0d4c7-121">说明</span><span class="sxs-lookup"><span data-stu-id="0d4c7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0d4c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d4c7-122">Authorization</span></span> | <span data-ttu-id="0d4c7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d4c7-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="0d4c7-125">Content-type</span></span> | <span data-ttu-id="0d4c7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0d4c7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d4c7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d4c7-128">Request body</span></span>

<span data-ttu-id="0d4c7-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0d4c7-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0d4c7-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d4c7-132">属性</span><span class="sxs-lookup"><span data-stu-id="0d4c7-132">Property</span></span>     | <span data-ttu-id="0d4c7-133">类型</span><span class="sxs-lookup"><span data-stu-id="0d4c7-133">Type</span></span>        | <span data-ttu-id="0d4c7-134">描述</span><span class="sxs-lookup"><span data-stu-id="0d4c7-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d4c7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0d4c7-135">displayName</span></span>|<span data-ttu-id="0d4c7-136">String</span><span class="sxs-lookup"><span data-stu-id="0d4c7-136">String</span></span>|<span data-ttu-id="0d4c7-137">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-137">Human-readable name of the location.</span></span>|
|<span data-ttu-id="0d4c7-138">ipRanges</span><span class="sxs-lookup"><span data-stu-id="0d4c7-138">ipRanges</span></span>|<span data-ttu-id="0d4c7-139">[ipRange](../resources/iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d4c7-139">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="0d4c7-140">来自 IETF RFC5962 的 IPv4 CIDR 格式（1.2.3.4/32）或任何允许的 IPv6 格式的 IP 地址范围列表。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-140">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="0d4c7-141">isTrusted</span><span class="sxs-lookup"><span data-stu-id="0d4c7-141">isTrusted</span></span>|<span data-ttu-id="0d4c7-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d4c7-142">Boolean</span></span>|<span data-ttu-id="0d4c7-143">如果此位置`true`是明确信任的，则该值为。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-143">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="0d4c7-144">响应</span><span class="sxs-lookup"><span data-stu-id="0d4c7-144">Response</span></span>

<span data-ttu-id="0d4c7-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d4c7-147">示例</span><span class="sxs-lookup"><span data-stu-id="0d4c7-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d4c7-148">请求</span><span class="sxs-lookup"><span data-stu-id="0d4c7-148">Request</span></span>

<span data-ttu-id="0d4c7-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-149">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0d4c7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d4c7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d4c7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d4c7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d4c7-152">响应</span><span class="sxs-lookup"><span data-stu-id="0d4c7-152">Response</span></span>

<span data-ttu-id="0d4c7-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-153">The following is an example of the response.</span></span>

> <span data-ttu-id="0d4c7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d4c7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
