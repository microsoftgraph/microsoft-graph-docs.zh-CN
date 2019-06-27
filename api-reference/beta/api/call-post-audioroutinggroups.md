---
title: 创建音频路由组
description: 创建新的**audioRoutingGroup**。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 05b7e7230857da139e7331940f014b20001f3b9b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262256"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="3ba58-103">创建音频路由组</span><span class="sxs-lookup"><span data-stu-id="3ba58-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ba58-104">创建新的**audioRoutingGroup**。</span><span class="sxs-lookup"><span data-stu-id="3ba58-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ba58-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ba58-105">Permissions</span></span>
<span data-ttu-id="3ba58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ba58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ba58-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ba58-108">Permission type</span></span>                        | <span data-ttu-id="3ba58-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ba58-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ba58-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ba58-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ba58-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ba58-111">Not supported.</span></span>                               |
| <span data-ttu-id="3ba58-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ba58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ba58-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ba58-113">Not supported.</span></span>                               |
| <span data-ttu-id="3ba58-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ba58-114">Application</span></span>                            | <span data-ttu-id="3ba58-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="3ba58-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ba58-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ba58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="3ba58-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ba58-117">Request headers</span></span>
| <span data-ttu-id="3ba58-118">名称</span><span class="sxs-lookup"><span data-stu-id="3ba58-118">Name</span></span>          | <span data-ttu-id="3ba58-119">说明</span><span class="sxs-lookup"><span data-stu-id="3ba58-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3ba58-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ba58-120">Authorization</span></span> | <span data-ttu-id="3ba58-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ba58-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ba58-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ba58-123">Request body</span></span>
<span data-ttu-id="3ba58-124">在请求正文中, 提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ba58-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ba58-125">响应</span><span class="sxs-lookup"><span data-stu-id="3ba58-125">Response</span></span>
<span data-ttu-id="3ba58-126">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3ba58-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ba58-127">示例</span><span class="sxs-lookup"><span data-stu-id="3ba58-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="3ba58-128">示例 1: 一对一音频路由组</span><span class="sxs-lookup"><span data-stu-id="3ba58-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="3ba58-129">请求</span><span class="sxs-lookup"><span data-stu-id="3ba58-129">Request</span></span>
<span data-ttu-id="3ba58-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ba58-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```

<span data-ttu-id="3ba58-131">在请求正文中, 提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ba58-131">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="3ba58-132">响应</span><span class="sxs-lookup"><span data-stu-id="3ba58-132">Response</span></span>

> <span data-ttu-id="3ba58-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ba58-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3ba58-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3ba58-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3ba58-136">C#</span><span class="sxs-lookup"><span data-stu-id="3ba58-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ba58-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ba58-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3ba58-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="3ba58-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-audioRoutingGroup-from-call-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="3ba58-139">示例 2: 多播 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="3ba58-139">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="3ba58-140">请求</span><span class="sxs-lookup"><span data-stu-id="3ba58-140">Request</span></span>
<span data-ttu-id="3ba58-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ba58-141">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233
```

<!-- {
  "blockType": "example",
  "name": "create-audioRoutingGroup-from-call",
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<span data-ttu-id="3ba58-142">在请求正文中, 提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ba58-142">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="3ba58-143">响应</span><span class="sxs-lookup"><span data-stu-id="3ba58-143">Response</span></span>

> <span data-ttu-id="3ba58-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ba58-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233
```
<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-post-audioroutinggroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
