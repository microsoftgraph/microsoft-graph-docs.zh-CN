---
title: 更新音频路由组
description: 修改 audioRoutingGroup 的源和接收器。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6e8bfe43529632988249206a0d84cc6e50e8324e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048006"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="6528b-103">更新音频路由组</span><span class="sxs-lookup"><span data-stu-id="6528b-103">Update audio routing group</span></span>

<span data-ttu-id="6528b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6528b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6528b-105">修改 [audioRoutingGroup 的源和接收器](../resources/audioroutinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="6528b-105">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6528b-106">权限</span><span class="sxs-lookup"><span data-stu-id="6528b-106">Permissions</span></span>
<span data-ttu-id="6528b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6528b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6528b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6528b-109">Permission type</span></span> | <span data-ttu-id="6528b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6528b-110">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="6528b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6528b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6528b-112">不支持</span><span class="sxs-lookup"><span data-stu-id="6528b-112">Not Supported</span></span>                       |
| <span data-ttu-id="6528b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6528b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6528b-114">不支持</span><span class="sxs-lookup"><span data-stu-id="6528b-114">Not Supported</span></span>                       |
| <span data-ttu-id="6528b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6528b-115">Application</span></span>     | <span data-ttu-id="6528b-116">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="6528b-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6528b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6528b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="6528b-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="6528b-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6528b-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="6528b-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6528b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6528b-120">Request headers</span></span>
| <span data-ttu-id="6528b-121">名称</span><span class="sxs-lookup"><span data-stu-id="6528b-121">Name</span></span>          | <span data-ttu-id="6528b-122">说明</span><span class="sxs-lookup"><span data-stu-id="6528b-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6528b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6528b-123">Authorization</span></span> | <span data-ttu-id="6528b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6528b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6528b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6528b-126">Request body</span></span>
<span data-ttu-id="6528b-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="6528b-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6528b-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="6528b-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6528b-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6528b-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6528b-130">属性</span><span class="sxs-lookup"><span data-stu-id="6528b-130">Property</span></span>       | <span data-ttu-id="6528b-131">类型</span><span class="sxs-lookup"><span data-stu-id="6528b-131">Type</span></span>    |<span data-ttu-id="6528b-132">说明</span><span class="sxs-lookup"><span data-stu-id="6528b-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6528b-133">receivers</span><span class="sxs-lookup"><span data-stu-id="6528b-133">receivers</span></span> | <span data-ttu-id="6528b-134">字符串集合</span><span class="sxs-lookup"><span data-stu-id="6528b-134">String collection</span></span> | <span data-ttu-id="6528b-135">audioRoutingGroup 中的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="6528b-135">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="6528b-136">routingMode</span><span class="sxs-lookup"><span data-stu-id="6528b-136">routingMode</span></span> | <span data-ttu-id="6528b-137">String</span><span class="sxs-lookup"><span data-stu-id="6528b-137">String</span></span> | <span data-ttu-id="6528b-138">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="6528b-138">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="6528b-139">源</span><span class="sxs-lookup"><span data-stu-id="6528b-139">sources</span></span> | <span data-ttu-id="6528b-140">字符串集合</span><span class="sxs-lookup"><span data-stu-id="6528b-140">String collection</span></span> | <span data-ttu-id="6528b-141">audioRoutingGroup 中的源参与者。</span><span class="sxs-lookup"><span data-stu-id="6528b-141">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="6528b-142">响应</span><span class="sxs-lookup"><span data-stu-id="6528b-142">Response</span></span>
<span data-ttu-id="6528b-143">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [audioRoutingGroup](../resources/audioroutinggroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6528b-143">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6528b-144">示例</span><span class="sxs-lookup"><span data-stu-id="6528b-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6528b-145">请求</span><span class="sxs-lookup"><span data-stu-id="6528b-145">Request</span></span>
<span data-ttu-id="6528b-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6528b-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6528b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6528b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="6528b-148">C#</span><span class="sxs-lookup"><span data-stu-id="6528b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6528b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6528b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6528b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6528b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6528b-151">Java</span><span class="sxs-lookup"><span data-stu-id="6528b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6528b-152">响应</span><span class="sxs-lookup"><span data-stu-id="6528b-152">Response</span></span>

> <span data-ttu-id="6528b-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6528b-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
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
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


