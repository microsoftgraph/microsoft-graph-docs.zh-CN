---
title: 获取 privilegedRoleSettings
description: 检索给定角色的角色设置。 将返回一个 privilegedRoleSettings 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 6fd8d585f8046d26f971f8598c797eb32e0b7df9
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374376"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="56a2e-104">获取 privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="56a2e-104">Get privilegedRoleSettings</span></span>

<span data-ttu-id="56a2e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56a2e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56a2e-106">检索给定角色的角色设置。</span><span class="sxs-lookup"><span data-stu-id="56a2e-106">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="56a2e-107">将返回一个 [privilegedRoleSettings](../resources/privilegedrolesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56a2e-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="56a2e-108">权限</span><span class="sxs-lookup"><span data-stu-id="56a2e-108">Permissions</span></span>

<span data-ttu-id="56a2e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56a2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="56a2e-111">请求者需要具有以下角色之一： _特权角色管理员_、 _全局管理员_、 _安全管理员_或 _安全读者_。</span><span class="sxs-lookup"><span data-stu-id="56a2e-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="56a2e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="56a2e-112">Permission type</span></span>      | <span data-ttu-id="56a2e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56a2e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56a2e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56a2e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="56a2e-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56a2e-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56a2e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56a2e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56a2e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="56a2e-117">Not supported.</span></span>    |
|<span data-ttu-id="56a2e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="56a2e-118">Application</span></span> | <span data-ttu-id="56a2e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="56a2e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56a2e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56a2e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56a2e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56a2e-121">Optional query parameters</span></span>
<span data-ttu-id="56a2e-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="56a2e-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56a2e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="56a2e-123">Request headers</span></span>
| <span data-ttu-id="56a2e-124">名称</span><span class="sxs-lookup"><span data-stu-id="56a2e-124">Name</span></span>      |<span data-ttu-id="56a2e-125">说明</span><span class="sxs-lookup"><span data-stu-id="56a2e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56a2e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="56a2e-126">Authorization</span></span>  | <span data-ttu-id="56a2e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56a2e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56a2e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="56a2e-129">Request body</span></span>
<span data-ttu-id="56a2e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56a2e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56a2e-131">响应</span><span class="sxs-lookup"><span data-stu-id="56a2e-131">Response</span></span>

<span data-ttu-id="56a2e-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [privilegedRoleSettings](../resources/privilegedrolesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56a2e-132">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="56a2e-133">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="56a2e-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="56a2e-134">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="56a2e-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="56a2e-135">示例</span><span class="sxs-lookup"><span data-stu-id="56a2e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56a2e-136">请求</span><span class="sxs-lookup"><span data-stu-id="56a2e-136">Request</span></span>
<span data-ttu-id="56a2e-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56a2e-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56a2e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="56a2e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="c"></a>[<span data-ttu-id="56a2e-139">C#</span><span class="sxs-lookup"><span data-stu-id="56a2e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56a2e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56a2e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56a2e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56a2e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="56a2e-142">响应</span><span class="sxs-lookup"><span data-stu-id="56a2e-142">Response</span></span>
<span data-ttu-id="56a2e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56a2e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
