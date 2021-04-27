---
title: 创建音频路由组
description: 创建新的 **audioRoutingGroup**。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f4c7cbc969b676db6786bf0d708e92381fd4cecf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047628"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="0358a-103">创建音频路由组</span><span class="sxs-lookup"><span data-stu-id="0358a-103">Create audio routing group</span></span>

<span data-ttu-id="0358a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0358a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0358a-105">创建新的 **audioRoutingGroup**。</span><span class="sxs-lookup"><span data-stu-id="0358a-105">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="0358a-106">权限</span><span class="sxs-lookup"><span data-stu-id="0358a-106">Permissions</span></span>
<span data-ttu-id="0358a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0358a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0358a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0358a-109">Permission type</span></span>                        | <span data-ttu-id="0358a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0358a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0358a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0358a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0358a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0358a-112">Not supported.</span></span>                               |
| <span data-ttu-id="0358a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0358a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0358a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0358a-114">Not supported.</span></span>                               |
| <span data-ttu-id="0358a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0358a-115">Application</span></span>                            | <span data-ttu-id="0358a-116">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="0358a-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0358a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0358a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="0358a-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="0358a-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="0358a-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="0358a-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0358a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0358a-120">Request headers</span></span>
| <span data-ttu-id="0358a-121">名称</span><span class="sxs-lookup"><span data-stu-id="0358a-121">Name</span></span>          | <span data-ttu-id="0358a-122">说明</span><span class="sxs-lookup"><span data-stu-id="0358a-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0358a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0358a-123">Authorization</span></span> | <span data-ttu-id="0358a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0358a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0358a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0358a-126">Request body</span></span>
<span data-ttu-id="0358a-127">在请求正文中，提供 [audioRoutingGroup](../resources/audioroutinggroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0358a-127">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0358a-128">响应</span><span class="sxs-lookup"><span data-stu-id="0358a-128">Response</span></span>
<span data-ttu-id="0358a-129">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [audioRoutingGroup](../resources/audioroutinggroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0358a-129">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0358a-130">示例</span><span class="sxs-lookup"><span data-stu-id="0358a-130">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="0358a-131">示例 1：一对一音频路由组</span><span class="sxs-lookup"><span data-stu-id="0358a-131">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="0358a-132">请求</span><span class="sxs-lookup"><span data-stu-id="0358a-132">Request</span></span>
<span data-ttu-id="0358a-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0358a-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0358a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0358a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
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
# <a name="c"></a>[<span data-ttu-id="0358a-135">C#</span><span class="sxs-lookup"><span data-stu-id="0358a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0358a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0358a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0358a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0358a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0358a-138">Java</span><span class="sxs-lookup"><span data-stu-id="0358a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-audioroutinggroup-from-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0358a-139">在请求正文中，提供 [audioRoutingGroup](../resources/audioroutinggroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0358a-139">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0358a-140">响应</span><span class="sxs-lookup"><span data-stu-id="0358a-140">Response</span></span>

> <span data-ttu-id="0358a-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0358a-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="0358a-142">示例 2：多播 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="0358a-142">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="0358a-143">请求</span><span class="sxs-lookup"><span data-stu-id="0358a-143">Request</span></span>
<span data-ttu-id="0358a-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0358a-144">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
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

<span data-ttu-id="0358a-145">在请求正文中，提供 [audioRoutingGroup](../resources/audioroutinggroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0358a-145">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0358a-146">响应</span><span class="sxs-lookup"><span data-stu-id="0358a-146">Response</span></span>

> <span data-ttu-id="0358a-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0358a-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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


