---
title: 获取音频路由组
description: 检索 audioRoutingGroup 对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2214726a474fc30fb2f1acf2f3c34c7eb4b9f39c
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792449"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="0425f-103">获取音频路由组</span><span class="sxs-lookup"><span data-stu-id="0425f-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0425f-104">检索[audioRoutingGroup](../resources/audioroutinggroup.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0425f-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0425f-105">权限</span><span class="sxs-lookup"><span data-stu-id="0425f-105">Permissions</span></span>
<span data-ttu-id="0425f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0425f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0425f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0425f-108">Permission type</span></span>                        | <span data-ttu-id="0425f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0425f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0425f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0425f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0425f-111">不支持</span><span class="sxs-lookup"><span data-stu-id="0425f-111">Not Supported</span></span>                               |
| <span data-ttu-id="0425f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0425f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0425f-113">不支持</span><span class="sxs-lookup"><span data-stu-id="0425f-113">Not Supported</span></span>                               |
| <span data-ttu-id="0425f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0425f-114">Application</span></span>                            | <span data-ttu-id="0425f-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="0425f-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0425f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0425f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0425f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0425f-117">Optional query parameters</span></span>
<span data-ttu-id="0425f-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0425f-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0425f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0425f-119">Request headers</span></span>
| <span data-ttu-id="0425f-120">名称</span><span class="sxs-lookup"><span data-stu-id="0425f-120">Name</span></span>          | <span data-ttu-id="0425f-121">说明</span><span class="sxs-lookup"><span data-stu-id="0425f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0425f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0425f-122">Authorization</span></span> | <span data-ttu-id="0425f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0425f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0425f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0425f-125">Request body</span></span>
<span data-ttu-id="0425f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0425f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0425f-127">响应</span><span class="sxs-lookup"><span data-stu-id="0425f-127">Response</span></span>
<span data-ttu-id="0425f-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0425f-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0425f-129">示例</span><span class="sxs-lookup"><span data-stu-id="0425f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0425f-130">请求</span><span class="sxs-lookup"><span data-stu-id="0425f-130">Request</span></span>
<span data-ttu-id="0425f-131">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0425f-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0425f-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0425f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0425f-133">C#</span><span class="sxs-lookup"><span data-stu-id="0425f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0425f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0425f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0425f-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="0425f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0425f-136">响应</span><span class="sxs-lookup"><span data-stu-id="0425f-136">Response</span></span>

> <span data-ttu-id="0425f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0425f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
