---
title: Get endpoint
description: 检索特定终结点对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: b4581105a06a7f234462e904822a3e87c52899f2
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459772"
---
# <a name="get-endpoint"></a><span data-ttu-id="5d741-103">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="5d741-103">Get endpoint</span></span>

<span data-ttu-id="5d741-104">检索特定 [终结点](../resources/endpoint.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5d741-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d741-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="5d741-105">Permissions</span></span>
<span data-ttu-id="5d741-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5d741-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d741-108">Permission type</span></span>      | <span data-ttu-id="5d741-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d741-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d741-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d741-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d741-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d741-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d741-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d741-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d741-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d741-113">Not supported.</span></span>    |
|<span data-ttu-id="5d741-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d741-114">Application</span></span> | <span data-ttu-id="5d741-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d741-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d741-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d741-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d741-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5d741-117">Optional query parameters</span></span>
<span data-ttu-id="5d741-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5d741-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d741-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d741-119">Request headers</span></span>
| <span data-ttu-id="5d741-120">名称</span><span class="sxs-lookup"><span data-stu-id="5d741-120">Name</span></span>      |<span data-ttu-id="5d741-121">说明</span><span class="sxs-lookup"><span data-stu-id="5d741-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d741-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d741-122">Authorization</span></span>  | <span data-ttu-id="5d741-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d741-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d741-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d741-125">Request body</span></span>
<span data-ttu-id="5d741-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d741-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d741-127">响应</span><span class="sxs-lookup"><span data-stu-id="5d741-127">Response</span></span>

<span data-ttu-id="5d741-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [终结点](../resources/endpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d741-128">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d741-129">示例</span><span class="sxs-lookup"><span data-stu-id="5d741-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d741-130">请求</span><span class="sxs-lookup"><span data-stu-id="5d741-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5d741-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d741-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="5d741-132">C#</span><span class="sxs-lookup"><span data-stu-id="5d741-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d741-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d741-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d741-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d741-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d741-135">响应</span><span class="sxs-lookup"><span data-stu-id="5d741-135">Response</span></span>
<span data-ttu-id="5d741-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5d741-136">Here is an example of the response.</span></span>
><span data-ttu-id="5d741-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d741-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
