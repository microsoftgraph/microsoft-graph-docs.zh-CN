---
title: 列出音频路由组
description: 检索**audioRoutingGroup**对象的列表。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: edb9b6caba0cca8e4788cafa6ce6ec1fd6f345ae
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006331"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="9834b-103">列出音频路由组</span><span class="sxs-lookup"><span data-stu-id="9834b-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9834b-104">检索**audioRoutingGroup**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9834b-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9834b-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="9834b-105">Permissions</span></span>
<span data-ttu-id="9834b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9834b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9834b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9834b-108">Permission type</span></span>                        | <span data-ttu-id="9834b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9834b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9834b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9834b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9834b-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="9834b-111">Not Supported.</span></span>                               |
| <span data-ttu-id="9834b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9834b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9834b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9834b-113">Not Supported.</span></span>                               |
| <span data-ttu-id="9834b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9834b-114">Application</span></span>     | <span data-ttu-id="9834b-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="9834b-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9834b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9834b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /communications/calls/{id}/audioRoutingGroups
```
> <span data-ttu-id="9834b-117">**注意：**`/app`路径已被弃用。</span><span class="sxs-lookup"><span data-stu-id="9834b-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="9834b-118">接下来，请使用`/communications`路径。</span><span class="sxs-lookup"><span data-stu-id="9834b-118">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="9834b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9834b-119">Optional query parameters</span></span>
<span data-ttu-id="9834b-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9834b-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9834b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9834b-121">Request headers</span></span>
| <span data-ttu-id="9834b-122">名称</span><span class="sxs-lookup"><span data-stu-id="9834b-122">Name</span></span>          | <span data-ttu-id="9834b-123">说明</span><span class="sxs-lookup"><span data-stu-id="9834b-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9834b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9834b-124">Authorization</span></span> | <span data-ttu-id="9834b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9834b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9834b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9834b-127">Request body</span></span>
<span data-ttu-id="9834b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9834b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9834b-129">响应</span><span class="sxs-lookup"><span data-stu-id="9834b-129">Response</span></span>
<span data-ttu-id="9834b-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9834b-130">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9834b-131">示例</span><span class="sxs-lookup"><span data-stu-id="9834b-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9834b-132">请求</span><span class="sxs-lookup"><span data-stu-id="9834b-132">Request</span></span>
<span data-ttu-id="9834b-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9834b-133">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9834b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9834b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9834b-135">C#</span><span class="sxs-lookup"><span data-stu-id="9834b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9834b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9834b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9834b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9834b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9834b-138">响应</span><span class="sxs-lookup"><span data-stu-id="9834b-138">Response</span></span>

> <span data-ttu-id="9834b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9834b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
