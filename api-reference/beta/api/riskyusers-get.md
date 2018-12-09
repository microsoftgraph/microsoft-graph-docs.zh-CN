---
title: 获取 riskyUsers
description: 检索的属性和**riskyUsers**对象的关系。
ms.openlocfilehash: 7212e99e53d990df9cd9fea7dae754a693edc745
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209682"
---
# <a name="get-riskyusers"></a><span data-ttu-id="d2ce9-103">获取 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d2ce9-103">Get riskyUsers</span></span>

> <span data-ttu-id="d2ce9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2ce9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2ce9-106">检索的属性和**riskyUsers**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2ce9-107">权限</span><span class="sxs-lookup"><span data-stu-id="d2ce9-107">Permissions</span></span>
<span data-ttu-id="d2ce9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2ce9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2ce9-110">Permission type</span></span>      | <span data-ttu-id="d2ce9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2ce9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2ce9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2ce9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2ce9-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2ce9-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="d2ce9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2ce9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2ce9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-115">Not supported.</span></span>    |
|<span data-ttu-id="d2ce9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2ce9-116">Application</span></span> | <span data-ttu-id="d2ce9-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2ce9-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2ce9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2ce9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="d2ce9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2ce9-119">Request headers</span></span>
| <span data-ttu-id="d2ce9-120">Name</span><span class="sxs-lookup"><span data-stu-id="d2ce9-120">Name</span></span>      |<span data-ttu-id="d2ce9-121">说明</span><span class="sxs-lookup"><span data-stu-id="d2ce9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2ce9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2ce9-122">Authorization</span></span>  | <span data-ttu-id="d2ce9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2ce9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2ce9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2ce9-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2ce9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2ce9-128">Request body</span></span>
<span data-ttu-id="d2ce9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2ce9-130">响应</span><span class="sxs-lookup"><span data-stu-id="d2ce9-130">Response</span></span>

<span data-ttu-id="d2ce9-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[riskyUser](../resources/riskyuser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2ce9-132">示例</span><span class="sxs-lookup"><span data-stu-id="d2ce9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2ce9-133">请求</span><span class="sxs-lookup"><span data-stu-id="d2ce9-133">Request</span></span>
<span data-ttu-id="d2ce9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="d2ce9-135">响应</span><span class="sxs-lookup"><span data-stu-id="d2ce9-135">Response</span></span>
<span data-ttu-id="d2ce9-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d2ce9-136">Here is an example of the response.</span></span>
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
