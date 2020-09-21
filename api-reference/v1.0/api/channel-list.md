---
title: 列出频道
description: 检索此团队中的频道列表。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8496383023781f796389bfbaf616bc0c64b9e97e
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843252"
---
# <a name="list-channels"></a><span data-ttu-id="1a8eb-103">列出频道</span><span class="sxs-lookup"><span data-stu-id="1a8eb-103">List channels</span></span>

<span data-ttu-id="1a8eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a8eb-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1a8eb-105">检索此团队中的[频道](../resources/channel.md)列表。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-105">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a8eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a8eb-106">Permissions</span></span>
<span data-ttu-id="1a8eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a8eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a8eb-109">Permission type</span></span>      | <span data-ttu-id="1a8eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a8eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a8eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a8eb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1a8eb-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8eb-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a8eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a8eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a8eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-114">Not supported.</span></span>    |
|<span data-ttu-id="1a8eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a8eb-115">Application</span></span> | <span data-ttu-id="1a8eb-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8eb-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="1a8eb-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1a8eb-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a8eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a8eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a8eb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a8eb-120">Optional query parameters</span></span>
<span data-ttu-id="1a8eb-121">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a8eb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a8eb-122">Request headers</span></span>
| <span data-ttu-id="1a8eb-123">标头</span><span class="sxs-lookup"><span data-stu-id="1a8eb-123">Header</span></span>       | <span data-ttu-id="1a8eb-124">值</span><span class="sxs-lookup"><span data-stu-id="1a8eb-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a8eb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a8eb-125">Authorization</span></span>  | <span data-ttu-id="1a8eb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a8eb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a8eb-128">Request body</span></span>
<span data-ttu-id="1a8eb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a8eb-130">响应</span><span class="sxs-lookup"><span data-stu-id="1a8eb-130">Response</span></span>

<span data-ttu-id="1a8eb-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Channel](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a8eb-132">示例</span><span class="sxs-lookup"><span data-stu-id="1a8eb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a8eb-133">请求</span><span class="sxs-lookup"><span data-stu-id="1a8eb-133">Request</span></span>
<span data-ttu-id="1a8eb-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a8eb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a8eb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels
```
# <a name="c"></a>[<span data-ttu-id="1a8eb-136">C#</span><span class="sxs-lookup"><span data-stu-id="1a8eb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a8eb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a8eb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a8eb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a8eb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a8eb-139">Java</span><span class="sxs-lookup"><span data-stu-id="1a8eb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a8eb-140">响应</span><span class="sxs-lookup"><span data-stu-id="1a8eb-140">Response</span></span>
<span data-ttu-id="1a8eb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a8eb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
