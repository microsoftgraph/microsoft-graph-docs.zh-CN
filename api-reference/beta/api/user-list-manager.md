---
title: 列出经理
description: 获取用户的经理。返回指定为用户经理的用户或联系人。
ms.openlocfilehash: 3601b7c13eb97b288cc65e927432bd420105970a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044126"
---
# <a name="list-manager"></a><span data-ttu-id="01594-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="01594-104">List manager</span></span>

> <span data-ttu-id="01594-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01594-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01594-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01594-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01594-p103">获取用户的经理。返回指定为用户经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="01594-p103">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="01594-109">权限</span><span class="sxs-lookup"><span data-stu-id="01594-109">Permissions</span></span>
<span data-ttu-id="01594-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01594-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01594-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="01594-112">Permission type</span></span>      | <span data-ttu-id="01594-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01594-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01594-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01594-114">Delegated (work or school account)</span></span> | <span data-ttu-id="01594-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01594-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01594-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01594-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01594-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="01594-117">Not supported.</span></span>    |
|<span data-ttu-id="01594-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="01594-118">Application</span></span> | <span data-ttu-id="01594-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01594-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01594-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01594-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01594-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01594-121">Optional query parameters</span></span>
<span data-ttu-id="01594-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="01594-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="01594-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="01594-123">Request headers</span></span>
| <span data-ttu-id="01594-124">标头</span><span class="sxs-lookup"><span data-stu-id="01594-124">Header</span></span>       | <span data-ttu-id="01594-125">值</span><span class="sxs-lookup"><span data-stu-id="01594-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="01594-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="01594-126">Authorization</span></span>  | <span data-ttu-id="01594-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01594-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01594-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01594-129">Content-Type</span></span>   | <span data-ttu-id="01594-130">application/json</span><span class="sxs-lookup"><span data-stu-id="01594-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01594-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="01594-131">Request body</span></span>
<span data-ttu-id="01594-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01594-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01594-133">响应</span><span class="sxs-lookup"><span data-stu-id="01594-133">Response</span></span>

<span data-ttu-id="01594-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01594-134">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01594-135">示例</span><span class="sxs-lookup"><span data-stu-id="01594-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01594-136">请求</span><span class="sxs-lookup"><span data-stu-id="01594-136">Request</span></span>
<span data-ttu-id="01594-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01594-137">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="01594-138">响应</span><span class="sxs-lookup"><span data-stu-id="01594-138">Response</span></span>
<span data-ttu-id="01594-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="01594-139">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
