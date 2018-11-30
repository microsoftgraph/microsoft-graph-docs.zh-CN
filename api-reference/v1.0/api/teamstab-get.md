---
title: 获取选项卡
description: '检索的属性和指定的选项卡的关系。 '
ms.openlocfilehash: 0a183d9bd55e0002a40335849549285d45fe9f69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007854"
---
# <a name="get-tab"></a><span data-ttu-id="1bc4e-103">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="1bc4e-103">Get tab</span></span>



<span data-ttu-id="1bc4e-104">检索的属性和指定的[选项卡](../resources/teamstab.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1bc4e-105">权限</span><span class="sxs-lookup"><span data-stu-id="1bc4e-105">Permissions</span></span>
<span data-ttu-id="1bc4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bc4e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bc4e-108">Permission type</span></span>      | <span data-ttu-id="1bc4e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bc4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bc4e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bc4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1bc4e-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc4e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1bc4e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bc4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc4e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-113">Not supported.</span></span>    |
|<span data-ttu-id="1bc4e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bc4e-114">Application</span></span> | <span data-ttu-id="1bc4e-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc4e-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="1bc4e-116">目前，仅[委派权限](/graph/permissions-reference)支持此操作。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-116">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="1bc4e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bc4e-117">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bc4e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1bc4e-118">Optional query parameters</span></span>

<span data-ttu-id="1bc4e-119">此方法支持 $select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-119">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bc4e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bc4e-120">Request headers</span></span>
| <span data-ttu-id="1bc4e-121">标头</span><span class="sxs-lookup"><span data-stu-id="1bc4e-121">Header</span></span>       | <span data-ttu-id="1bc4e-122">值</span><span class="sxs-lookup"><span data-stu-id="1bc4e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bc4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bc4e-123">Authorization</span></span>  | <span data-ttu-id="1bc4e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bc4e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bc4e-126">Request body</span></span>
<span data-ttu-id="1bc4e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bc4e-128">响应</span><span class="sxs-lookup"><span data-stu-id="1bc4e-128">Response</span></span>

<span data-ttu-id="1bc4e-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[选项卡](../resources/teamstab.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-129">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bc4e-130">示例</span><span class="sxs-lookup"><span data-stu-id="1bc4e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1bc4e-131">请求</span><span class="sxs-lookup"><span data-stu-id="1bc4e-131">Request</span></span>
<span data-ttu-id="1bc4e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-132">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="1bc4e-133">响应</span><span class="sxs-lookup"><span data-stu-id="1bc4e-133">Response</span></span>
<span data-ttu-id="1bc4e-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-134">The following is an example of the response.</span></span> 

><span data-ttu-id="1bc4e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1bc4e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
