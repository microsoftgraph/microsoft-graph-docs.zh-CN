---
title: 创建音频路由组
description: 创建新的**audioRoutingGroup**。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 38fa18f34ee457be395c39b0894d1e90828ec772
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944458"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="63b11-103">创建音频路由组</span><span class="sxs-lookup"><span data-stu-id="63b11-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63b11-104">创建新的**audioRoutingGroup**。</span><span class="sxs-lookup"><span data-stu-id="63b11-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="63b11-105">权限</span><span class="sxs-lookup"><span data-stu-id="63b11-105">Permissions</span></span>
<span data-ttu-id="63b11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63b11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63b11-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="63b11-108">Permission type</span></span>                        | <span data-ttu-id="63b11-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63b11-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63b11-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63b11-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="63b11-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="63b11-111">Not supported.</span></span>                               |
| <span data-ttu-id="63b11-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63b11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63b11-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="63b11-113">Not supported.</span></span>                               |
| <span data-ttu-id="63b11-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="63b11-114">Application</span></span>                            | <span data-ttu-id="63b11-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="63b11-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63b11-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63b11-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="63b11-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="63b11-117">Request headers</span></span>
| <span data-ttu-id="63b11-118">名称</span><span class="sxs-lookup"><span data-stu-id="63b11-118">Name</span></span>          | <span data-ttu-id="63b11-119">说明</span><span class="sxs-lookup"><span data-stu-id="63b11-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="63b11-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="63b11-120">Authorization</span></span> | <span data-ttu-id="63b11-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63b11-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63b11-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="63b11-123">Request body</span></span>
<span data-ttu-id="63b11-124">在请求正文中, 提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63b11-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="63b11-125">响应</span><span class="sxs-lookup"><span data-stu-id="63b11-125">Response</span></span>
<span data-ttu-id="63b11-126">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63b11-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63b11-127">示例</span><span class="sxs-lookup"><span data-stu-id="63b11-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="63b11-128">示例 1: 一对一音频路由组</span><span class="sxs-lookup"><span data-stu-id="63b11-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="63b11-129">请求</span><span class="sxs-lookup"><span data-stu-id="63b11-129">Request</span></span>
<span data-ttu-id="63b11-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="63b11-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="63b11-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="63b11-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="63b11-132">C#</span><span class="sxs-lookup"><span data-stu-id="63b11-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63b11-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="63b11-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63b11-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="63b11-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="63b11-135">Java</span><span class="sxs-lookup"><span data-stu-id="63b11-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-audioroutinggroup-from-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="63b11-136">在请求正文中, 提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63b11-136">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="63b11-137">响应</span><span class="sxs-lookup"><span data-stu-id="63b11-137">Response</span></span>

> <span data-ttu-id="63b11-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63b11-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="63b11-140">示例 2: 多播 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="63b11-140">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="63b11-141">请求</span><span class="sxs-lookup"><span data-stu-id="63b11-141">Request</span></span>
<span data-ttu-id="63b11-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="63b11-142">The following example shows the request.</span></span>

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

<span data-ttu-id="63b11-143">在请求正文中, 提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63b11-143">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="63b11-144">响应</span><span class="sxs-lookup"><span data-stu-id="63b11-144">Response</span></span>

> <span data-ttu-id="63b11-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63b11-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
