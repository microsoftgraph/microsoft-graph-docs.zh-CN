---
title: 列出音频路由组
description: 检索**audioRoutingGroup**对象的列表。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a782af2bb7690cc55dd3a4632aeb0cf93734da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461257"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="fb4b8-103">列出音频路由组</span><span class="sxs-lookup"><span data-stu-id="fb4b8-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb4b8-104">检索**audioRoutingGroup**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb4b8-105">权限</span><span class="sxs-lookup"><span data-stu-id="fb4b8-105">Permissions</span></span>
<span data-ttu-id="fb4b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb4b8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb4b8-108">Permission type</span></span>                        | <span data-ttu-id="fb4b8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb4b8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fb4b8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb4b8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb4b8-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-111">Not Supported.</span></span>                               |
| <span data-ttu-id="fb4b8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb4b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb4b8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-113">Not Supported.</span></span>                               |
| <span data-ttu-id="fb4b8-114">应用</span><span class="sxs-lookup"><span data-stu-id="fb4b8-114">Application</span></span>     | <span data-ttu-id="fb4b8-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="fb4b8-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb4b8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb4b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb4b8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb4b8-117">Optional query parameters</span></span>
<span data-ttu-id="fb4b8-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb4b8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb4b8-119">Request headers</span></span>
| <span data-ttu-id="fb4b8-120">名称</span><span class="sxs-lookup"><span data-stu-id="fb4b8-120">Name</span></span>          | <span data-ttu-id="fb4b8-121">说明</span><span class="sxs-lookup"><span data-stu-id="fb4b8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fb4b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb4b8-122">Authorization</span></span> | <span data-ttu-id="fb4b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb4b8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb4b8-125">Request body</span></span>
<span data-ttu-id="fb4b8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb4b8-127">响应</span><span class="sxs-lookup"><span data-stu-id="fb4b8-127">Response</span></span>
<span data-ttu-id="fb4b8-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[audioRoutingGroup](../resources/audioroutinggroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-128">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb4b8-129">示例</span><span class="sxs-lookup"><span data-stu-id="fb4b8-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fb4b8-130">请求</span><span class="sxs-lookup"><span data-stu-id="fb4b8-130">Request</span></span>
<span data-ttu-id="fb4b8-131">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="fb4b8-132">响应</span><span class="sxs-lookup"><span data-stu-id="fb4b8-132">Response</span></span>

> <span data-ttu-id="fb4b8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fb4b8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
