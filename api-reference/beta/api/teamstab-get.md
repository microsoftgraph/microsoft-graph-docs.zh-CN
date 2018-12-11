---
title: 获取选项卡
description: '检索的属性和指定的选项卡的关系。 '
ms.openlocfilehash: 7bef495fbb37a878a291f2aac6004d386e932cbd
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222406"
---
# <a name="get-tab"></a><span data-ttu-id="0006f-103">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="0006f-103">Get tab</span></span>

> <span data-ttu-id="0006f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0006f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0006f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0006f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0006f-106">检索的属性和指定的[选项卡](../resources/teamstab.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="0006f-106">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0006f-107">权限</span><span class="sxs-lookup"><span data-stu-id="0006f-107">Permissions</span></span>
<span data-ttu-id="0006f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0006f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0006f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0006f-110">Permission type</span></span>      | <span data-ttu-id="0006f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0006f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0006f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0006f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0006f-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0006f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0006f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0006f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0006f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0006f-115">Not supported.</span></span>    |
|<span data-ttu-id="0006f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0006f-116">Application</span></span> | <span data-ttu-id="0006f-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0006f-117">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="0006f-118">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0006f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0006f-119">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="0006f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0006f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0006f-120">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0006f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0006f-121">Optional query parameters</span></span>

<span data-ttu-id="0006f-122">此方法支持 $select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="0006f-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0006f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0006f-123">Request headers</span></span>
| <span data-ttu-id="0006f-124">标头</span><span class="sxs-lookup"><span data-stu-id="0006f-124">Header</span></span>       | <span data-ttu-id="0006f-125">值</span><span class="sxs-lookup"><span data-stu-id="0006f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0006f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0006f-126">Authorization</span></span>  | <span data-ttu-id="0006f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0006f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0006f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0006f-129">Request body</span></span>
<span data-ttu-id="0006f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0006f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0006f-131">响应</span><span class="sxs-lookup"><span data-stu-id="0006f-131">Response</span></span>

<span data-ttu-id="0006f-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[选项卡](../resources/teamstab.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0006f-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0006f-133">示例</span><span class="sxs-lookup"><span data-stu-id="0006f-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0006f-134">请求</span><span class="sxs-lookup"><span data-stu-id="0006f-134">Request</span></span>
<span data-ttu-id="0006f-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0006f-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="0006f-136">响应</span><span class="sxs-lookup"><span data-stu-id="0006f-136">Response</span></span>
<span data-ttu-id="0006f-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0006f-137">The following is an example of the response.</span></span> 

><span data-ttu-id="0006f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0006f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
