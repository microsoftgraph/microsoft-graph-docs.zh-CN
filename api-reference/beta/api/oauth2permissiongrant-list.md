---
title: 列出 oAuth2PermissionGrants
description: 检索表示委派权限授予的 oauth2PermissionGrant 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 3e42b422a358a0fc513a2b11014e74f91432ecfc
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231932"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="ccf5d-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="ccf5d-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="ccf5d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccf5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccf5d-105">检索 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象的列表，这些对象代表已授予客户端应用程序代表登录用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

> [!NOTE]
> <span data-ttu-id="ccf5d-106">此请求可能有最近创建、更新或删除的委派权限授予的复制延迟。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-106">This request might have replication delays for delegated permission grants that were recently created, updated, or deleted.</span></span> <span data-ttu-id="ccf5d-107">如果指定了筛选，此延迟 `clientId` 将最小化。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-107">This delay will be minimized if a filter on `clientId` is specified.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccf5d-108">权限</span><span class="sxs-lookup"><span data-stu-id="ccf5d-108">Permissions</span></span>

<span data-ttu-id="ccf5d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccf5d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccf5d-111">Permission type</span></span>      | <span data-ttu-id="ccf5d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccf5d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccf5d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccf5d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ccf5d-114">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ccf5d-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ccf5d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccf5d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccf5d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-116">Not supported.</span></span>    |
|<span data-ttu-id="ccf5d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccf5d-117">Application</span></span> | <span data-ttu-id="ccf5d-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccf5d-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccf5d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccf5d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccf5d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ccf5d-120">Optional query parameters</span></span>

<span data-ttu-id="ccf5d-121">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccf5d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccf5d-122">Request headers</span></span>

| <span data-ttu-id="ccf5d-123">名称</span><span class="sxs-lookup"><span data-stu-id="ccf5d-123">Name</span></span> | <span data-ttu-id="ccf5d-124">说明</span><span class="sxs-lookup"><span data-stu-id="ccf5d-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ccf5d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccf5d-125">Authorization</span></span>  | <span data-ttu-id="ccf5d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccf5d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccf5d-128">Request body</span></span>

<span data-ttu-id="ccf5d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccf5d-130">响应</span><span class="sxs-lookup"><span data-stu-id="ccf5d-130">Response</span></span>

<span data-ttu-id="ccf5d-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccf5d-132">示例</span><span class="sxs-lookup"><span data-stu-id="ccf5d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccf5d-133">请求</span><span class="sxs-lookup"><span data-stu-id="ccf5d-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ccf5d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccf5d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="ccf5d-135">C#</span><span class="sxs-lookup"><span data-stu-id="ccf5d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccf5d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccf5d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccf5d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccf5d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccf5d-138">Java</span><span class="sxs-lookup"><span data-stu-id="ccf5d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ccf5d-139">响应</span><span class="sxs-lookup"><span data-stu-id="ccf5d-139">Response</span></span>

> <span data-ttu-id="ccf5d-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ccf5d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value",
      "expiryTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


