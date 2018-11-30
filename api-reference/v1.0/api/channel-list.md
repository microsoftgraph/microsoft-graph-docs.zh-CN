---
title: 列表通道
description: 检索此团队中的通道的列表。
ms.openlocfilehash: 5f96d4c47a787839626a9d90733d087906407b01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009084"
---
# <a name="list-channels"></a><span data-ttu-id="29421-103">列表通道</span><span class="sxs-lookup"><span data-stu-id="29421-103">List channels</span></span>



<span data-ttu-id="29421-104">检索此团队中的[通道](../resources/channel.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="29421-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="29421-105">权限</span><span class="sxs-lookup"><span data-stu-id="29421-105">Permissions</span></span>
<span data-ttu-id="29421-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="29421-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="29421-108">Permission type</span></span>      | <span data-ttu-id="29421-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29421-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29421-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29421-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29421-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29421-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="29421-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29421-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29421-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="29421-113">Not supported.</span></span>    |
|<span data-ttu-id="29421-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="29421-114">Application</span></span> | <span data-ttu-id="29421-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29421-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="29421-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29421-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29421-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="29421-117">Optional query parameters</span></span>
<span data-ttu-id="29421-118">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="29421-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29421-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="29421-119">Request headers</span></span>
| <span data-ttu-id="29421-120">标头</span><span class="sxs-lookup"><span data-stu-id="29421-120">Header</span></span>       | <span data-ttu-id="29421-121">值</span><span class="sxs-lookup"><span data-stu-id="29421-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29421-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29421-122">Authorization</span></span>  | <span data-ttu-id="29421-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29421-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29421-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="29421-125">Request body</span></span>
<span data-ttu-id="29421-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29421-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29421-127">响应</span><span class="sxs-lookup"><span data-stu-id="29421-127">Response</span></span>

<span data-ttu-id="29421-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[通道](../resources/channel.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="29421-128">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29421-129">示例</span><span class="sxs-lookup"><span data-stu-id="29421-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29421-130">请求</span><span class="sxs-lookup"><span data-stu-id="29421-130">Request</span></span>
<span data-ttu-id="29421-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29421-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="29421-132">响应</span><span class="sxs-lookup"><span data-stu-id="29421-132">Response</span></span>
<span data-ttu-id="29421-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29421-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
