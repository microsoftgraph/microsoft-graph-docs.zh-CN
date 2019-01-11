---
title: 列表通道
description: 检索此团队中的通道的列表。
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 23763e83f7e2e0d9333d39ebe439f8702b180f71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813522"
---
# <a name="list-channels"></a><span data-ttu-id="8efe4-103">列表通道</span><span class="sxs-lookup"><span data-stu-id="8efe4-103">List channels</span></span>

> <span data-ttu-id="8efe4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8efe4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8efe4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8efe4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8efe4-106">检索此团队中的[通道](../resources/channel.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="8efe4-106">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="8efe4-107">权限</span><span class="sxs-lookup"><span data-stu-id="8efe4-107">Permissions</span></span>
<span data-ttu-id="8efe4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8efe4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8efe4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8efe4-110">Permission type</span></span>      | <span data-ttu-id="8efe4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8efe4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8efe4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8efe4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8efe4-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8efe4-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8efe4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8efe4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8efe4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8efe4-115">Not supported.</span></span>    |
|<span data-ttu-id="8efe4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8efe4-116">Application</span></span> | <span data-ttu-id="8efe4-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8efe4-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8efe4-118">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="8efe4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8efe4-119">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="8efe4-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8efe4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8efe4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8efe4-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8efe4-121">Optional query parameters</span></span>
<span data-ttu-id="8efe4-122">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="8efe4-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8efe4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="8efe4-123">Request headers</span></span>
| <span data-ttu-id="8efe4-124">标头</span><span class="sxs-lookup"><span data-stu-id="8efe4-124">Header</span></span>       | <span data-ttu-id="8efe4-125">值</span><span class="sxs-lookup"><span data-stu-id="8efe4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8efe4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8efe4-126">Authorization</span></span>  | <span data-ttu-id="8efe4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8efe4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8efe4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8efe4-129">Request body</span></span>
<span data-ttu-id="8efe4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8efe4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8efe4-131">响应</span><span class="sxs-lookup"><span data-stu-id="8efe4-131">Response</span></span>

<span data-ttu-id="8efe4-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[通道](../resources/channel.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="8efe4-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8efe4-133">示例</span><span class="sxs-lookup"><span data-stu-id="8efe4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8efe4-134">请求</span><span class="sxs-lookup"><span data-stu-id="8efe4-134">Request</span></span>
<span data-ttu-id="8efe4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8efe4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="8efe4-136">响应</span><span class="sxs-lookup"><span data-stu-id="8efe4-136">Response</span></span>
<span data-ttu-id="8efe4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8efe4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
