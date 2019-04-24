---
title: 列出频道
description: 检索此团队中的频道列表。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 47e284bb5eb89c88a961dc82f802fd6eac083310
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456547"
---
# <a name="list-channels"></a><span data-ttu-id="69753-103">列出频道</span><span class="sxs-lookup"><span data-stu-id="69753-103">List channels</span></span>



<span data-ttu-id="69753-104">检索此团队中的[频道](../resources/channel.md)列表。</span><span class="sxs-lookup"><span data-stu-id="69753-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="69753-105">权限</span><span class="sxs-lookup"><span data-stu-id="69753-105">Permissions</span></span>
<span data-ttu-id="69753-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="69753-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="69753-108">Permission type</span></span>      | <span data-ttu-id="69753-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69753-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69753-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69753-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69753-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69753-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69753-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69753-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69753-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="69753-113">Not supported.</span></span>    |
|<span data-ttu-id="69753-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="69753-114">Application</span></span> | <span data-ttu-id="69753-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69753-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="69753-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="69753-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="69753-117">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="69753-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="69753-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69753-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69753-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69753-119">Optional query parameters</span></span>
<span data-ttu-id="69753-120">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69753-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69753-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="69753-121">Request headers</span></span>
| <span data-ttu-id="69753-122">标头</span><span class="sxs-lookup"><span data-stu-id="69753-122">Header</span></span>       | <span data-ttu-id="69753-123">值</span><span class="sxs-lookup"><span data-stu-id="69753-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69753-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="69753-124">Authorization</span></span>  | <span data-ttu-id="69753-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69753-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69753-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69753-127">Request body</span></span>
<span data-ttu-id="69753-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69753-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69753-129">响应</span><span class="sxs-lookup"><span data-stu-id="69753-129">Response</span></span>

<span data-ttu-id="69753-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Channel](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="69753-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69753-131">示例</span><span class="sxs-lookup"><span data-stu-id="69753-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69753-132">请求</span><span class="sxs-lookup"><span data-stu-id="69753-132">Request</span></span>
<span data-ttu-id="69753-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69753-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="69753-134">响应</span><span class="sxs-lookup"><span data-stu-id="69753-134">Response</span></span>
<span data-ttu-id="69753-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69753-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
