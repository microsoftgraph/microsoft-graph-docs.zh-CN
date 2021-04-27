---
title: 获取 privilegedRoleSettings
description: 检索给定角色的角色设置。 将返回 privilegedRoleSettings 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 73c2a01c171ec39f2702b5bf9ce6a3138a93456b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052885"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="08ebc-104">获取 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="08ebc-104">Get privilegedRoleSettings</span></span>

<span data-ttu-id="08ebc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08ebc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08ebc-106">检索给定角色的角色设置。</span><span class="sxs-lookup"><span data-stu-id="08ebc-106">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="08ebc-107">将 [返回 privilegedRoleSettings](../resources/privilegedrolesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08ebc-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="08ebc-108">权限</span><span class="sxs-lookup"><span data-stu-id="08ebc-108">Permissions</span></span>

<span data-ttu-id="08ebc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08ebc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="08ebc-111">请求程序需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="08ebc-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="08ebc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="08ebc-112">Permission type</span></span>      | <span data-ttu-id="08ebc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08ebc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08ebc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08ebc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="08ebc-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08ebc-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08ebc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08ebc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08ebc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="08ebc-117">Not supported.</span></span>    |
|<span data-ttu-id="08ebc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="08ebc-118">Application</span></span> | <span data-ttu-id="08ebc-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="08ebc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08ebc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08ebc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08ebc-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="08ebc-121">Optional query parameters</span></span>
<span data-ttu-id="08ebc-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="08ebc-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08ebc-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="08ebc-123">Request headers</span></span>
| <span data-ttu-id="08ebc-124">名称</span><span class="sxs-lookup"><span data-stu-id="08ebc-124">Name</span></span>      |<span data-ttu-id="08ebc-125">说明</span><span class="sxs-lookup"><span data-stu-id="08ebc-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08ebc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="08ebc-126">Authorization</span></span>  | <span data-ttu-id="08ebc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08ebc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08ebc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="08ebc-129">Request body</span></span>
<span data-ttu-id="08ebc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08ebc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ebc-131">响应</span><span class="sxs-lookup"><span data-stu-id="08ebc-131">Response</span></span>

<span data-ttu-id="08ebc-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [privilegedRoleSettings](../resources/privilegedrolesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08ebc-132">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="08ebc-133">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="08ebc-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="08ebc-134">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="08ebc-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="08ebc-135">示例</span><span class="sxs-lookup"><span data-stu-id="08ebc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08ebc-136">请求</span><span class="sxs-lookup"><span data-stu-id="08ebc-136">Request</span></span>
<span data-ttu-id="08ebc-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08ebc-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08ebc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="08ebc-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="c"></a>[<span data-ttu-id="08ebc-139">C#</span><span class="sxs-lookup"><span data-stu-id="08ebc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08ebc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08ebc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08ebc-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08ebc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08ebc-142">Java</span><span class="sxs-lookup"><span data-stu-id="08ebc-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="08ebc-143">响应</span><span class="sxs-lookup"><span data-stu-id="08ebc-143">Response</span></span>
<span data-ttu-id="08ebc-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="08ebc-144">Here is an example of the response.</span></span> <span data-ttu-id="08ebc-145">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="08ebc-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "2016-10-19T10:37:00Z",
  "maxElavationDuration": "2016-10-19T10:37:00Z",
  "elevationDuration": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
