---
title: 获取音频路由组
description: 检索 audioRoutingGroup 对象的属性和关系。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a597ce800d709df1ce5b0eb4ab54f8f2028605e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441324"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="0e040-103">获取音频路由组</span><span class="sxs-lookup"><span data-stu-id="0e040-103">Get audio routing group</span></span>

<span data-ttu-id="0e040-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0e040-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e040-105">检索[audioRoutingGroup](../resources/audioroutinggroup.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e040-105">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e040-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e040-106">Permissions</span></span>
<span data-ttu-id="0e040-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e040-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e040-109">Permission type</span></span>                        | <span data-ttu-id="0e040-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e040-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e040-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e040-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e040-112">不支持</span><span class="sxs-lookup"><span data-stu-id="0e040-112">Not Supported</span></span>                               |
| <span data-ttu-id="0e040-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e040-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e040-114">不支持</span><span class="sxs-lookup"><span data-stu-id="0e040-114">Not Supported</span></span>                               |
| <span data-ttu-id="0e040-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e040-115">Application</span></span>                            | <span data-ttu-id="0e040-116">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="0e040-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e040-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e040-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="0e040-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="0e040-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="0e040-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="0e040-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="0e040-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e040-120">Optional query parameters</span></span>
<span data-ttu-id="0e040-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e040-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e040-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e040-122">Request headers</span></span>
| <span data-ttu-id="0e040-123">名称</span><span class="sxs-lookup"><span data-stu-id="0e040-123">Name</span></span>          | <span data-ttu-id="0e040-124">说明</span><span class="sxs-lookup"><span data-stu-id="0e040-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0e040-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e040-125">Authorization</span></span> | <span data-ttu-id="0e040-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e040-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e040-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e040-128">Request body</span></span>
<span data-ttu-id="0e040-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e040-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e040-130">响应</span><span class="sxs-lookup"><span data-stu-id="0e040-130">Response</span></span>
<span data-ttu-id="0e040-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e040-131">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e040-132">示例</span><span class="sxs-lookup"><span data-stu-id="0e040-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0e040-133">请求</span><span class="sxs-lookup"><span data-stu-id="0e040-133">Request</span></span>
<span data-ttu-id="0e040-134">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e040-134">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e040-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e040-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="0e040-136">C#</span><span class="sxs-lookup"><span data-stu-id="0e040-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e040-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e040-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e040-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e040-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e040-139">响应</span><span class="sxs-lookup"><span data-stu-id="0e040-139">Response</span></span>

> <span data-ttu-id="0e040-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0e040-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
