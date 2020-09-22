---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 178da2aee1dcc25dbd29a32c2041f6d8150caed6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016875"
---
# <a name="list-manager"></a><span data-ttu-id="a95d4-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="a95d4-104">List manager</span></span>

<span data-ttu-id="a95d4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a95d4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a95d4-106">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="a95d4-106">Get user's manager.</span></span> <span data-ttu-id="a95d4-107">返回指定为用户经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="a95d4-107">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="a95d4-108">权限</span><span class="sxs-lookup"><span data-stu-id="a95d4-108">Permissions</span></span>
<span data-ttu-id="a95d4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a95d4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a95d4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a95d4-111">Permission type</span></span>      | <span data-ttu-id="a95d4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a95d4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a95d4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a95d4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a95d4-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a95d4-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a95d4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a95d4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a95d4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a95d4-116">Not supported.</span></span>    |
|<span data-ttu-id="a95d4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a95d4-117">Application</span></span> | <span data-ttu-id="a95d4-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a95d4-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a95d4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a95d4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a95d4-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a95d4-120">Optional query parameters</span></span>
<span data-ttu-id="a95d4-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a95d4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a95d4-122">请求头</span><span class="sxs-lookup"><span data-stu-id="a95d4-122">Request headers</span></span>
| <span data-ttu-id="a95d4-123">标头</span><span class="sxs-lookup"><span data-stu-id="a95d4-123">Header</span></span>       | <span data-ttu-id="a95d4-124">值</span><span class="sxs-lookup"><span data-stu-id="a95d4-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a95d4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a95d4-125">Authorization</span></span>  | <span data-ttu-id="a95d4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a95d4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a95d4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a95d4-128">Content-Type</span></span>   | <span data-ttu-id="a95d4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a95d4-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a95d4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a95d4-130">Request body</span></span>
<span data-ttu-id="a95d4-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a95d4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a95d4-132">响应</span><span class="sxs-lookup"><span data-stu-id="a95d4-132">Response</span></span>

<span data-ttu-id="a95d4-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a95d4-133">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a95d4-134">示例</span><span class="sxs-lookup"><span data-stu-id="a95d4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a95d4-135">请求</span><span class="sxs-lookup"><span data-stu-id="a95d4-135">Request</span></span>
<span data-ttu-id="a95d4-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a95d4-136">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="a95d4-137">响应</span><span class="sxs-lookup"><span data-stu-id="a95d4-137">Response</span></span>
<span data-ttu-id="a95d4-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a95d4-138">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->


