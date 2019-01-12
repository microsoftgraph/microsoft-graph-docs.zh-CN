---
title: 创建音频路由组
description: 创建新**audioRoutingGroup**。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe623a581233324e13c949d16570b1396fdd663c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966382"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="f6f47-103">创建音频路由组</span><span class="sxs-lookup"><span data-stu-id="f6f47-103">Create audio routing group</span></span>

> <span data-ttu-id="f6f47-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f6f47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6f47-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6f47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6f47-106">创建新**audioRoutingGroup**。</span><span class="sxs-lookup"><span data-stu-id="f6f47-106">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6f47-107">权限</span><span class="sxs-lookup"><span data-stu-id="f6f47-107">Permissions</span></span>
<span data-ttu-id="f6f47-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6f47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6f47-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6f47-110">Permission type</span></span>                        | <span data-ttu-id="f6f47-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6f47-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f6f47-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6f47-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6f47-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6f47-113">Not supported.</span></span>                               |
| <span data-ttu-id="f6f47-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6f47-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6f47-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6f47-115">Not supported.</span></span>                               |
| <span data-ttu-id="f6f47-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6f47-116">Application</span></span>                            | <span data-ttu-id="f6f47-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="f6f47-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6f47-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6f47-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="f6f47-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6f47-119">Request headers</span></span>
| <span data-ttu-id="f6f47-120">名称</span><span class="sxs-lookup"><span data-stu-id="f6f47-120">Name</span></span>          | <span data-ttu-id="f6f47-121">说明</span><span class="sxs-lookup"><span data-stu-id="f6f47-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f6f47-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6f47-122">Authorization</span></span> | <span data-ttu-id="f6f47-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6f47-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6f47-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6f47-125">Request body</span></span>
<span data-ttu-id="f6f47-126">在请求正文中，提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6f47-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f6f47-127">响应</span><span class="sxs-lookup"><span data-stu-id="f6f47-127">Response</span></span>
<span data-ttu-id="f6f47-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f6f47-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6f47-129">示例</span><span class="sxs-lookup"><span data-stu-id="f6f47-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="f6f47-130">示例 1： 一对一音频路由组</span><span class="sxs-lookup"><span data-stu-id="f6f47-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="f6f47-131">请求</span><span class="sxs-lookup"><span data-stu-id="f6f47-131">Request</span></span>
<span data-ttu-id="f6f47-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6f47-132">The following example shows the request.</span></span>

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

<span data-ttu-id="f6f47-133">在请求正文中，提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6f47-133">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f6f47-134">响应</span><span class="sxs-lookup"><span data-stu-id="f6f47-134">Response</span></span>

> <span data-ttu-id="f6f47-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f6f47-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="f6f47-137">示例 2： 多播的 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="f6f47-137">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="f6f47-138">请求</span><span class="sxs-lookup"><span data-stu-id="f6f47-138">Request</span></span>
<span data-ttu-id="f6f47-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6f47-139">The following example shows the request.</span></span>

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

<span data-ttu-id="f6f47-140">在请求正文中，提供[audioRoutingGroup](../resources/audioroutinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6f47-140">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f6f47-141">响应</span><span class="sxs-lookup"><span data-stu-id="f6f47-141">Response</span></span>

> <span data-ttu-id="f6f47-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f6f47-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
