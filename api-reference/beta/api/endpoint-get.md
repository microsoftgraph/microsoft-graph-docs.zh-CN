---
title: 获取终结点
description: 检索的属性和特定的终结点对象的关系。
ms.openlocfilehash: fe5e820f18a22762436d8558d501d0250a090aa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042627"
---
# <a name="get-endpoint"></a><span data-ttu-id="05910-103">获取终结点</span><span class="sxs-lookup"><span data-stu-id="05910-103">Get endpoint</span></span>

> <span data-ttu-id="05910-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="05910-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05910-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="05910-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05910-106">检索的属性和特定[终结点](../resources/endpoint.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="05910-106">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="05910-107">权限</span><span class="sxs-lookup"><span data-stu-id="05910-107">Permissions</span></span>
<span data-ttu-id="05910-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05910-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05910-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="05910-110">Permission type</span></span>      | <span data-ttu-id="05910-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05910-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05910-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05910-112">Delegated (work or school account)</span></span> | <span data-ttu-id="05910-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05910-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="05910-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05910-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05910-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="05910-115">Not supported.</span></span>    |
|<span data-ttu-id="05910-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="05910-116">Application</span></span> | <span data-ttu-id="05910-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05910-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05910-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05910-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05910-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="05910-119">Optional query parameters</span></span>
<span data-ttu-id="05910-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="05910-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05910-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="05910-121">Request headers</span></span>
| <span data-ttu-id="05910-122">名称</span><span class="sxs-lookup"><span data-stu-id="05910-122">Name</span></span>      |<span data-ttu-id="05910-123">说明</span><span class="sxs-lookup"><span data-stu-id="05910-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05910-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="05910-124">Authorization</span></span>  | <span data-ttu-id="05910-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05910-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="05910-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05910-127">Content-Type</span></span>   | <span data-ttu-id="05910-128">Application/Json</span><span class="sxs-lookup"><span data-stu-id="05910-128">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="05910-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="05910-129">Request body</span></span>
<span data-ttu-id="05910-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05910-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05910-131">响应</span><span class="sxs-lookup"><span data-stu-id="05910-131">Response</span></span>

<span data-ttu-id="05910-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[终结点](../resources/endpoint.md)对象。</span><span class="sxs-lookup"><span data-stu-id="05910-132">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05910-133">示例</span><span class="sxs-lookup"><span data-stu-id="05910-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05910-134">请求</span><span class="sxs-lookup"><span data-stu-id="05910-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="05910-135">响应</span><span class="sxs-lookup"><span data-stu-id="05910-135">Response</span></span>
<span data-ttu-id="05910-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05910-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->