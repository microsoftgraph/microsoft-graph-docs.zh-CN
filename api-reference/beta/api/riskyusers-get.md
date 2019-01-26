---
title: 获取 riskyUsers
description: 检索的属性和**riskyUsers**对象的关系。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 18798df27ebccb3e56afa4e0f479ced4b4029863
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575298"
---
# <a name="get-riskyusers"></a><span data-ttu-id="c7b82-103">获取 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c7b82-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7b82-104">检索的属性和**riskyUsers**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c7b82-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="c7b82-105">**注意：** 此 API 要求的 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="c7b82-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7b82-106">权限</span><span class="sxs-lookup"><span data-stu-id="c7b82-106">Permissions</span></span>
<span data-ttu-id="c7b82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7b82-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7b82-109">Permission type</span></span>      | <span data-ttu-id="c7b82-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7b82-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7b82-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b82-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7b82-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7b82-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="c7b82-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7b82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7b82-114">Not supported.</span></span>    |
|<span data-ttu-id="c7b82-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7b82-115">Application</span></span> | <span data-ttu-id="c7b82-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7b82-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7b82-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7b82-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="c7b82-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7b82-118">Request headers</span></span>
| <span data-ttu-id="c7b82-119">名称</span><span class="sxs-lookup"><span data-stu-id="c7b82-119">Name</span></span>      |<span data-ttu-id="c7b82-120">说明</span><span class="sxs-lookup"><span data-stu-id="c7b82-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7b82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7b82-121">Authorization</span></span>  | <span data-ttu-id="c7b82-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7b82-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7b82-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c7b82-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7b82-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c7b82-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7b82-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7b82-127">Request body</span></span>
<span data-ttu-id="c7b82-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7b82-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7b82-129">响应</span><span class="sxs-lookup"><span data-stu-id="c7b82-129">Response</span></span>

<span data-ttu-id="c7b82-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[riskyUser](../resources/riskyuser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7b82-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7b82-131">示例</span><span class="sxs-lookup"><span data-stu-id="c7b82-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7b82-132">请求</span><span class="sxs-lookup"><span data-stu-id="c7b82-132">Request</span></span>
<span data-ttu-id="c7b82-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7b82-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
##### <a name="response"></a><span data-ttu-id="c7b82-134">响应</span><span class="sxs-lookup"><span data-stu-id="c7b82-134">Response</span></span>
<span data-ttu-id="c7b82-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c7b82-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": true,
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
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
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
