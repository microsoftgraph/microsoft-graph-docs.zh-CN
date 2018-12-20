---
title: 获取音频路由组
description: 检索的属性和 audioRoutingGroup 对象的关系。
author: VinodRavichandran
ms.openlocfilehash: 5f9a7771f31350dc30ed96e9eb81b40cc855b380
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380427"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="f432e-103">获取音频路由组</span><span class="sxs-lookup"><span data-stu-id="f432e-103">Get audio routing group</span></span>

> <span data-ttu-id="f432e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f432e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f432e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f432e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f432e-106">检索的属性和[audioRoutingGroup](../resources/audioroutinggroup.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f432e-106">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f432e-107">权限</span><span class="sxs-lookup"><span data-stu-id="f432e-107">Permissions</span></span>
<span data-ttu-id="f432e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f432e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f432e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f432e-110">Permission type</span></span>                        | <span data-ttu-id="f432e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f432e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f432e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f432e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f432e-113">不支持</span><span class="sxs-lookup"><span data-stu-id="f432e-113">Not Supported</span></span>                               |
| <span data-ttu-id="f432e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f432e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f432e-115">不支持</span><span class="sxs-lookup"><span data-stu-id="f432e-115">Not Supported</span></span>                               |
| <span data-ttu-id="f432e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f432e-116">Application</span></span>                            | <span data-ttu-id="f432e-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="f432e-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f432e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f432e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f432e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f432e-119">Optional query parameters</span></span>
<span data-ttu-id="f432e-120">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="f432e-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f432e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f432e-121">Request headers</span></span>
| <span data-ttu-id="f432e-122">名称</span><span class="sxs-lookup"><span data-stu-id="f432e-122">Name</span></span>          | <span data-ttu-id="f432e-123">说明</span><span class="sxs-lookup"><span data-stu-id="f432e-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f432e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f432e-124">Authorization</span></span> | <span data-ttu-id="f432e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f432e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f432e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f432e-127">Request body</span></span>
<span data-ttu-id="f432e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f432e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f432e-129">响应</span><span class="sxs-lookup"><span data-stu-id="f432e-129">Response</span></span>
<span data-ttu-id="f432e-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f432e-130">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f432e-131">示例</span><span class="sxs-lookup"><span data-stu-id="f432e-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f432e-132">请求</span><span class="sxs-lookup"><span data-stu-id="f432e-132">Request</span></span>
<span data-ttu-id="f432e-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f432e-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="f432e-134">响应</span><span class="sxs-lookup"><span data-stu-id="f432e-134">Response</span></span>

> <span data-ttu-id="f432e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f432e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
