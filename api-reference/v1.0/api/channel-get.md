---
title: 获取通道
description: 检索的属性和频道的关系。
ms.openlocfilehash: 42f25d0866af9000cfb6f96952ac19e32af0e87c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008419"
---
# <a name="get-channel"></a><span data-ttu-id="947bb-103">获取通道</span><span class="sxs-lookup"><span data-stu-id="947bb-103">Get channel</span></span>



<span data-ttu-id="947bb-104">检索的属性和[频道](../resources/channel.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="947bb-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="947bb-105">权限</span><span class="sxs-lookup"><span data-stu-id="947bb-105">Permissions</span></span>
<span data-ttu-id="947bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="947bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="947bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="947bb-108">Permission type</span></span>      | <span data-ttu-id="947bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="947bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="947bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="947bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="947bb-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="947bb-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="947bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="947bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="947bb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="947bb-113">Not supported.</span></span>    |
|<span data-ttu-id="947bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="947bb-114">Application</span></span> | <span data-ttu-id="947bb-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="947bb-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="947bb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="947bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="947bb-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="947bb-117">Optional query parameters</span></span>

<span data-ttu-id="947bb-118">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="947bb-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="947bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="947bb-119">Request headers</span></span>
| <span data-ttu-id="947bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="947bb-120">Header</span></span>       | <span data-ttu-id="947bb-121">值</span><span class="sxs-lookup"><span data-stu-id="947bb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="947bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="947bb-122">Authorization</span></span>  | <span data-ttu-id="947bb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="947bb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="947bb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="947bb-125">Request body</span></span>
<span data-ttu-id="947bb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="947bb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="947bb-127">响应</span><span class="sxs-lookup"><span data-stu-id="947bb-127">Response</span></span>

<span data-ttu-id="947bb-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[通道](../resources/channel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="947bb-128">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="947bb-129">示例</span><span class="sxs-lookup"><span data-stu-id="947bb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="947bb-130">请求</span><span class="sxs-lookup"><span data-stu-id="947bb-130">Request</span></span>
<span data-ttu-id="947bb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="947bb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="947bb-132">响应</span><span class="sxs-lookup"><span data-stu-id="947bb-132">Response</span></span>
<span data-ttu-id="947bb-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="947bb-133">Here is an example of the response.</span></span> 

><span data-ttu-id="947bb-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="947bb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
