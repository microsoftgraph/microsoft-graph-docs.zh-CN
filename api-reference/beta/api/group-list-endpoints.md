---
title: 列出终结点
description: 检索的终结点对象的列表。
author: dkershaw10
ms.openlocfilehash: d455cb8a5d1fb07a3d97cea376d9e2e49266892d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315944"
---
# <a name="list-endpoints"></a><span data-ttu-id="5a281-103">列出终结点</span><span class="sxs-lookup"><span data-stu-id="5a281-103">List endpoints</span></span>

> <span data-ttu-id="5a281-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a281-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a281-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a281-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a281-106">检索的[终结点](../resources/endpoint.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5a281-106">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a281-107">权限</span><span class="sxs-lookup"><span data-stu-id="5a281-107">Permissions</span></span>
<span data-ttu-id="5a281-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a281-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a281-110">Permission type</span></span>      | <span data-ttu-id="5a281-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a281-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a281-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a281-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a281-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a281-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a281-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a281-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a281-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a281-115">Not supported.</span></span>    |
|<span data-ttu-id="5a281-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a281-116">Application</span></span> | <span data-ttu-id="5a281-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a281-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a281-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a281-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a281-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a281-119">Optional query parameters</span></span>
<span data-ttu-id="5a281-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5a281-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a281-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a281-121">Request headers</span></span>
| <span data-ttu-id="5a281-122">Name</span><span class="sxs-lookup"><span data-stu-id="5a281-122">Name</span></span>      |<span data-ttu-id="5a281-123">说明</span><span class="sxs-lookup"><span data-stu-id="5a281-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a281-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a281-124">Authorization</span></span>  | <span data-ttu-id="5a281-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a281-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5a281-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a281-127">Content-Type</span></span>   | <span data-ttu-id="5a281-128">Application/Json</span><span class="sxs-lookup"><span data-stu-id="5a281-128">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a281-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a281-129">Request body</span></span>
<span data-ttu-id="5a281-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a281-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a281-131">响应</span><span class="sxs-lookup"><span data-stu-id="5a281-131">Response</span></span>

<span data-ttu-id="5a281-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[终结点](../resources/endpoint.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5a281-132">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a281-133">示例</span><span class="sxs-lookup"><span data-stu-id="5a281-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a281-134">请求</span><span class="sxs-lookup"><span data-stu-id="5a281-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="5a281-135">响应</span><span class="sxs-lookup"><span data-stu-id="5a281-135">Response</span></span>
<span data-ttu-id="5a281-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a281-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->