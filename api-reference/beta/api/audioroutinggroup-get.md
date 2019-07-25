---
title: 获取音频路由组
description: 检索 audioRoutingGroup 对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8d551fa292e746c77d1034025918e672668f1831
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856910"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="f1cf1-103">获取音频路由组</span><span class="sxs-lookup"><span data-stu-id="f1cf1-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1cf1-104">检索[audioRoutingGroup](../resources/audioroutinggroup.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1cf1-105">权限</span><span class="sxs-lookup"><span data-stu-id="f1cf1-105">Permissions</span></span>
<span data-ttu-id="f1cf1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1cf1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1cf1-108">Permission type</span></span>                        | <span data-ttu-id="f1cf1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1cf1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1cf1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1cf1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1cf1-111">不支持</span><span class="sxs-lookup"><span data-stu-id="f1cf1-111">Not Supported</span></span>                               |
| <span data-ttu-id="f1cf1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1cf1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1cf1-113">不支持</span><span class="sxs-lookup"><span data-stu-id="f1cf1-113">Not Supported</span></span>                               |
| <span data-ttu-id="f1cf1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1cf1-114">Application</span></span>                            | <span data-ttu-id="f1cf1-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="f1cf1-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1cf1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1cf1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1cf1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f1cf1-117">Optional query parameters</span></span>
<span data-ttu-id="f1cf1-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1cf1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1cf1-119">Request headers</span></span>
| <span data-ttu-id="f1cf1-120">名称</span><span class="sxs-lookup"><span data-stu-id="f1cf1-120">Name</span></span>          | <span data-ttu-id="f1cf1-121">说明</span><span class="sxs-lookup"><span data-stu-id="f1cf1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f1cf1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1cf1-122">Authorization</span></span> | <span data-ttu-id="f1cf1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1cf1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1cf1-125">Request body</span></span>
<span data-ttu-id="f1cf1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1cf1-127">响应</span><span class="sxs-lookup"><span data-stu-id="f1cf1-127">Response</span></span>
<span data-ttu-id="f1cf1-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1cf1-129">示例</span><span class="sxs-lookup"><span data-stu-id="f1cf1-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f1cf1-130">请求</span><span class="sxs-lookup"><span data-stu-id="f1cf1-130">Request</span></span>
<span data-ttu-id="f1cf1-131">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f1cf1-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f1cf1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1cf1-133">C#</span><span class="sxs-lookup"><span data-stu-id="f1cf1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1cf1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1cf1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1cf1-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="f1cf1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f1cf1-136">Java</span><span class="sxs-lookup"><span data-stu-id="f1cf1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f1cf1-137">响应</span><span class="sxs-lookup"><span data-stu-id="f1cf1-137">Response</span></span>

> <span data-ttu-id="f1cf1-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f1cf1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
