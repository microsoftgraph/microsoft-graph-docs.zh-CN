---
title: 列表 riskyUsers
description: 检索的属性和**riskyUsers**对象的关系。
ms.openlocfilehash: 152171ff098bb58e8cbb247ca687841e77594ead
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049462"
---
# <a name="list-riskyusers"></a><span data-ttu-id="e0dad-103">列表 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e0dad-103">List riskyUsers</span></span>

> <span data-ttu-id="e0dad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e0dad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0dad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0dad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0dad-106">检索的属性和**riskyUsers**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e0dad-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0dad-107">权限</span><span class="sxs-lookup"><span data-stu-id="e0dad-107">Permissions</span></span>
<span data-ttu-id="e0dad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0dad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0dad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0dad-110">Permission type</span></span>      | <span data-ttu-id="e0dad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0dad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0dad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0dad-113">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0dad-113">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="e0dad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0dad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0dad-115">Not supported.</span></span>    |
|<span data-ttu-id="e0dad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0dad-116">Application</span></span> | <span data-ttu-id="e0dad-117">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0dad-117">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0dad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0dad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0dad-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e0dad-119">Optional query parameters</span></span>
<span data-ttu-id="e0dad-120">此方法支持`$filter`自定义的查询响应。</span><span class="sxs-lookup"><span data-stu-id="e0dad-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="e0dad-121">请参阅本主题后面的示例。</span><span class="sxs-lookup"><span data-stu-id="e0dad-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e0dad-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0dad-122">Request headers</span></span>
| <span data-ttu-id="e0dad-123">名称</span><span class="sxs-lookup"><span data-stu-id="e0dad-123">Name</span></span>      |<span data-ttu-id="e0dad-124">说明</span><span class="sxs-lookup"><span data-stu-id="e0dad-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0dad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0dad-125">Authorization</span></span>  | <span data-ttu-id="e0dad-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0dad-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0dad-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0dad-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0dad-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e0dad-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0dad-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0dad-131">Request body</span></span>
<span data-ttu-id="e0dad-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0dad-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0dad-133">响应</span><span class="sxs-lookup"><span data-stu-id="e0dad-133">Response</span></span>

<span data-ttu-id="e0dad-134">如果成功，此方法返回`200 OK`响应正文中的响应代码和[identityRiskEvent](../resources/identityriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0dad-134">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0dad-135">示例</span><span class="sxs-lookup"><span data-stu-id="e0dad-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e0dad-136">请求 1</span><span class="sxs-lookup"><span data-stu-id="e0dad-136">Request 1</span></span>
<span data-ttu-id="e0dad-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0dad-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="e0dad-138">响应 1</span><span class="sxs-lookup"><span data-stu-id="e0dad-138">Response 1</span></span>
<span data-ttu-id="e0dad-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0dad-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
##### <a name="request-2"></a><span data-ttu-id="e0dad-140">请求 2</span><span class="sxs-lookup"><span data-stu-id="e0dad-140">Request 2</span></span>
<span data-ttu-id="e0dad-141">下面的示例演示如何使用`$filter`若要获取的 riskyUser 集合其聚合风险级别为 Medium。</span><span class="sxs-lookup"><span data-stu-id="e0dad-141">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="e0dad-142">响应 2</span><span class="sxs-lookup"><span data-stu-id="e0dad-142">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
      "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
      "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
      "isGuest": false,
      "isDeleted": false,
      "riskDetail": "none",
      "riskLevel": "medium",
      "riskState": "atRisk",
      "userDisplayName": "Jon Doe",
      "userPrincipalName": "jon@contoso.com",
      }
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
