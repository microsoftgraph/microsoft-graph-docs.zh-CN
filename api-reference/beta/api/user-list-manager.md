---
title: 列出经理
description: 获取用户的经理。返回指定为用户经理的用户或联系人。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87f57712bbef74864b6100527391d9f3c56f8455
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516096"
---
# <a name="list-manager"></a><span data-ttu-id="7ac07-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="7ac07-104">List manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ac07-p102">获取用户的经理。返回指定为用户经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="7ac07-p102">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ac07-107">权限</span><span class="sxs-lookup"><span data-stu-id="7ac07-107">Permissions</span></span>
<span data-ttu-id="7ac07-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ac07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac07-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ac07-110">Permission type</span></span>      | <span data-ttu-id="7ac07-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ac07-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ac07-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac07-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ac07-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ac07-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ac07-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ac07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ac07-115">Not supported.</span></span>    |
|<span data-ttu-id="7ac07-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ac07-116">Application</span></span> | <span data-ttu-id="7ac07-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac07-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ac07-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ac07-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ac07-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7ac07-119">Optional query parameters</span></span>
<span data-ttu-id="7ac07-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7ac07-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7ac07-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ac07-121">Request headers</span></span>
| <span data-ttu-id="7ac07-122">标头</span><span class="sxs-lookup"><span data-stu-id="7ac07-122">Header</span></span>       | <span data-ttu-id="7ac07-123">值</span><span class="sxs-lookup"><span data-stu-id="7ac07-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="7ac07-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ac07-124">Authorization</span></span>  | <span data-ttu-id="7ac07-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ac07-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ac07-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ac07-127">Content-Type</span></span>   | <span data-ttu-id="7ac07-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac07-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ac07-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ac07-129">Request body</span></span>
<span data-ttu-id="7ac07-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ac07-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ac07-131">响应</span><span class="sxs-lookup"><span data-stu-id="7ac07-131">Response</span></span>

<span data-ttu-id="7ac07-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ac07-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ac07-133">示例</span><span class="sxs-lookup"><span data-stu-id="7ac07-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ac07-134">请求</span><span class="sxs-lookup"><span data-stu-id="7ac07-134">Request</span></span>
<span data-ttu-id="7ac07-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ac07-135">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="7ac07-136">响应</span><span class="sxs-lookup"><span data-stu-id="7ac07-136">Response</span></span>
<span data-ttu-id="7ac07-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7ac07-137">Here is an example of the response.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
