---
title: 获取 riskyUsers
description: 检索的属性和**riskyUsers**对象的关系。
localization_priority: Normal
ms.openlocfilehash: da26be10b5a1aa631bd55f977ead806ed89c1406
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891124"
---
# <a name="get-riskyusers"></a><span data-ttu-id="ccc22-103">获取 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ccc22-103">Get riskyUsers</span></span>

> <span data-ttu-id="ccc22-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ccc22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccc22-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ccc22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccc22-106">检索的属性和**riskyUsers**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ccc22-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="ccc22-107">**注意：** 此 API 要求的 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="ccc22-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc22-108">权限</span><span class="sxs-lookup"><span data-stu-id="ccc22-108">Permissions</span></span>
<span data-ttu-id="ccc22-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccc22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccc22-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccc22-111">Permission type</span></span>      | <span data-ttu-id="ccc22-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccc22-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccc22-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc22-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ccc22-114">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccc22-114">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="ccc22-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc22-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccc22-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc22-116">Not supported.</span></span>    |
|<span data-ttu-id="ccc22-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccc22-117">Application</span></span> | <span data-ttu-id="ccc22-118">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccc22-118">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccc22-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccc22-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="ccc22-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccc22-120">Request headers</span></span>
| <span data-ttu-id="ccc22-121">名称</span><span class="sxs-lookup"><span data-stu-id="ccc22-121">Name</span></span>      |<span data-ttu-id="ccc22-122">说明</span><span class="sxs-lookup"><span data-stu-id="ccc22-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ccc22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc22-123">Authorization</span></span>  | <span data-ttu-id="ccc22-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccc22-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccc22-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ccc22-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="ccc22-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ccc22-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc22-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccc22-129">Request body</span></span>
<span data-ttu-id="ccc22-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccc22-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccc22-131">响应</span><span class="sxs-lookup"><span data-stu-id="ccc22-131">Response</span></span>

<span data-ttu-id="ccc22-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[riskyUser](../resources/riskyuser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ccc22-132">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ccc22-133">示例</span><span class="sxs-lookup"><span data-stu-id="ccc22-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccc22-134">请求</span><span class="sxs-lookup"><span data-stu-id="ccc22-134">Request</span></span>
<span data-ttu-id="ccc22-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ccc22-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="ccc22-136">响应</span><span class="sxs-lookup"><span data-stu-id="ccc22-136">Response</span></span>
<span data-ttu-id="ccc22-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ccc22-137">Here is an example of the response.</span></span>
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
