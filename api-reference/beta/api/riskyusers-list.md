---
title: 列表 riskyUsers
description: 检索的属性和**riskyUsers**对象的关系。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 5c0c0557a5cd84312ef9d6381d8cf3018ab8ce7d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519316"
---
# <a name="list-riskyusers"></a><span data-ttu-id="dcdfb-103">列表 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="dcdfb-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcdfb-104">检索的属性和**riskyUsers**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="dcdfb-105">**注意：** 此 API 要求的 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcdfb-106">权限</span><span class="sxs-lookup"><span data-stu-id="dcdfb-106">Permissions</span></span>
<span data-ttu-id="dcdfb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcdfb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcdfb-109">Permission type</span></span>      | <span data-ttu-id="dcdfb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcdfb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcdfb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcdfb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dcdfb-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcdfb-112">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="dcdfb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcdfb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcdfb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-114">Not supported.</span></span>    |
|<span data-ttu-id="dcdfb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcdfb-115">Application</span></span> | <span data-ttu-id="dcdfb-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcdfb-116">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcdfb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcdfb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dcdfb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dcdfb-118">Optional query parameters</span></span>
<span data-ttu-id="dcdfb-119">此方法支持`$filter`自定义的查询响应。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="dcdfb-120">请参阅本主题后面的示例。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="dcdfb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcdfb-121">Request headers</span></span>
| <span data-ttu-id="dcdfb-122">名称</span><span class="sxs-lookup"><span data-stu-id="dcdfb-122">Name</span></span>      |<span data-ttu-id="dcdfb-123">说明</span><span class="sxs-lookup"><span data-stu-id="dcdfb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcdfb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcdfb-124">Authorization</span></span>  | <span data-ttu-id="dcdfb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcdfb-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dcdfb-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="dcdfb-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcdfb-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcdfb-130">Request body</span></span>
<span data-ttu-id="dcdfb-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcdfb-132">响应</span><span class="sxs-lookup"><span data-stu-id="dcdfb-132">Response</span></span>

<span data-ttu-id="dcdfb-133">如果成功，此方法返回`200 OK`响应正文中的响应代码和[identityRiskEvent](../resources/identityriskevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-133">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dcdfb-134">示例</span><span class="sxs-lookup"><span data-stu-id="dcdfb-134">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="dcdfb-135">请求 1</span><span class="sxs-lookup"><span data-stu-id="dcdfb-135">Request 1</span></span>
<span data-ttu-id="dcdfb-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="dcdfb-137">响应 1</span><span class="sxs-lookup"><span data-stu-id="dcdfb-137">Response 1</span></span>
<span data-ttu-id="dcdfb-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-138">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="dcdfb-139">请求 2</span><span class="sxs-lookup"><span data-stu-id="dcdfb-139">Request 2</span></span>
<span data-ttu-id="dcdfb-140">下面的示例演示如何使用`$filter`若要获取的 riskyUser 集合其聚合风险级别为 Medium。</span><span class="sxs-lookup"><span data-stu-id="dcdfb-140">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="dcdfb-141">响应 2</span><span class="sxs-lookup"><span data-stu-id="dcdfb-141">Response 2</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
