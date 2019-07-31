---
title: 更新音频路由组
description: 修改 audioRoutingGroup 的源和接收器。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b99feecbd10a1d50551972a7d7b7dc38275f97a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945296"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="594e2-103">更新音频路由组</span><span class="sxs-lookup"><span data-stu-id="594e2-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="594e2-104">修改[audioRoutingGroup](../resources/audioroutinggroup.md)的源和接收器。</span><span class="sxs-lookup"><span data-stu-id="594e2-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="594e2-105">权限</span><span class="sxs-lookup"><span data-stu-id="594e2-105">Permissions</span></span>
<span data-ttu-id="594e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="594e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="594e2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="594e2-108">Permission type</span></span> | <span data-ttu-id="594e2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="594e2-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="594e2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="594e2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="594e2-111">不支持</span><span class="sxs-lookup"><span data-stu-id="594e2-111">Not Supported</span></span>                       |
| <span data-ttu-id="594e2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="594e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="594e2-113">不支持</span><span class="sxs-lookup"><span data-stu-id="594e2-113">Not Supported</span></span>                       |
| <span data-ttu-id="594e2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="594e2-114">Application</span></span>     | <span data-ttu-id="594e2-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="594e2-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="594e2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="594e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="594e2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="594e2-117">Request headers</span></span>
| <span data-ttu-id="594e2-118">名称</span><span class="sxs-lookup"><span data-stu-id="594e2-118">Name</span></span>          | <span data-ttu-id="594e2-119">说明</span><span class="sxs-lookup"><span data-stu-id="594e2-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="594e2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="594e2-120">Authorization</span></span> | <span data-ttu-id="594e2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="594e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="594e2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="594e2-123">Request body</span></span>
<span data-ttu-id="594e2-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="594e2-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="594e2-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="594e2-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="594e2-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="594e2-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="594e2-127">属性</span><span class="sxs-lookup"><span data-stu-id="594e2-127">Property</span></span>       | <span data-ttu-id="594e2-128">类型</span><span class="sxs-lookup"><span data-stu-id="594e2-128">Type</span></span>    |<span data-ttu-id="594e2-129">说明</span><span class="sxs-lookup"><span data-stu-id="594e2-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="594e2-130">接收器</span><span class="sxs-lookup"><span data-stu-id="594e2-130">receivers</span></span> | <span data-ttu-id="594e2-131">String collection</span><span class="sxs-lookup"><span data-stu-id="594e2-131">String collection</span></span> | <span data-ttu-id="594e2-132">AudioRoutingGroup 中的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="594e2-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="594e2-133">routingMode</span><span class="sxs-lookup"><span data-stu-id="594e2-133">routingMode</span></span> | <span data-ttu-id="594e2-134">String</span><span class="sxs-lookup"><span data-stu-id="594e2-134">String</span></span> | <span data-ttu-id="594e2-135">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="594e2-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="594e2-136">源</span><span class="sxs-lookup"><span data-stu-id="594e2-136">sources</span></span> | <span data-ttu-id="594e2-137">String collection</span><span class="sxs-lookup"><span data-stu-id="594e2-137">String collection</span></span> | <span data-ttu-id="594e2-138">AudioRoutingGroup 中的源参与者。</span><span class="sxs-lookup"><span data-stu-id="594e2-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="594e2-139">响应</span><span class="sxs-lookup"><span data-stu-id="594e2-139">Response</span></span>
<span data-ttu-id="594e2-140">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="594e2-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="594e2-141">示例</span><span class="sxs-lookup"><span data-stu-id="594e2-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="594e2-142">请求</span><span class="sxs-lookup"><span data-stu-id="594e2-142">Request</span></span>
<span data-ttu-id="594e2-143">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="594e2-143">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="594e2-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="594e2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json
Content-Length: 233

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
# <a name="ctabcsharp"></a>[<span data-ttu-id="594e2-145">C#</span><span class="sxs-lookup"><span data-stu-id="594e2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="594e2-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="594e2-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="594e2-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="594e2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="594e2-148">Java</span><span class="sxs-lookup"><span data-stu-id="594e2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="594e2-149">响应</span><span class="sxs-lookup"><span data-stu-id="594e2-149">Response</span></span>

> <span data-ttu-id="594e2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="594e2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
