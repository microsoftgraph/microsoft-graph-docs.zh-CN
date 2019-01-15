---
title: 获取通道
description: 检索的属性和频道的关系。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 5b5f70b79deaf7fa90b6083dcbd4c83a09aa84e5
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016651"
---
# <a name="get-channel"></a><span data-ttu-id="2c29e-103">获取通道</span><span class="sxs-lookup"><span data-stu-id="2c29e-103">Get channel</span></span>



<span data-ttu-id="2c29e-104">检索的属性和[频道](../resources/channel.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="2c29e-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c29e-105">权限</span><span class="sxs-lookup"><span data-stu-id="2c29e-105">Permissions</span></span>
<span data-ttu-id="2c29e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c29e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c29e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c29e-108">Permission type</span></span>      | <span data-ttu-id="2c29e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c29e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c29e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c29e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c29e-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c29e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c29e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c29e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c29e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c29e-113">Not supported.</span></span>    |
|<span data-ttu-id="2c29e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c29e-114">Application</span></span> | <span data-ttu-id="2c29e-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c29e-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="2c29e-116">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="2c29e-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2c29e-117">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="2c29e-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2c29e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c29e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c29e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c29e-119">Optional query parameters</span></span>

<span data-ttu-id="2c29e-120">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="2c29e-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c29e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c29e-121">Request headers</span></span>
| <span data-ttu-id="2c29e-122">标头</span><span class="sxs-lookup"><span data-stu-id="2c29e-122">Header</span></span>       | <span data-ttu-id="2c29e-123">值</span><span class="sxs-lookup"><span data-stu-id="2c29e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c29e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c29e-124">Authorization</span></span>  | <span data-ttu-id="2c29e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c29e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c29e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c29e-127">Request body</span></span>
<span data-ttu-id="2c29e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c29e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c29e-129">响应</span><span class="sxs-lookup"><span data-stu-id="2c29e-129">Response</span></span>

<span data-ttu-id="2c29e-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[通道](../resources/channel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c29e-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c29e-131">示例</span><span class="sxs-lookup"><span data-stu-id="2c29e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c29e-132">请求</span><span class="sxs-lookup"><span data-stu-id="2c29e-132">Request</span></span>
<span data-ttu-id="2c29e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c29e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="2c29e-134">响应</span><span class="sxs-lookup"><span data-stu-id="2c29e-134">Response</span></span>
<span data-ttu-id="2c29e-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2c29e-135">Here is an example of the response.</span></span> 

><span data-ttu-id="2c29e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2c29e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
