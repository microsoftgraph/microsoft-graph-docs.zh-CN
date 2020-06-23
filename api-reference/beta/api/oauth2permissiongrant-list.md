---
title: 列出 oAuth2PermissionGrants
description: 检索 oauth2PermissionGrant 对象的列表，表示委派权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 2b6ecf8c40f4f9a41608ef7f6edf588c1032839c
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845496"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="c1755-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="c1755-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="c1755-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1755-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1755-105">检索[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象的列表，这些对象代表已为客户端应用程序授予的代表登录用户访问 api 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="c1755-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1755-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c1755-106">Permissions</span></span>

<span data-ttu-id="c1755-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c1755-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c1755-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1755-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1755-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1755-109">Permission type</span></span>      | <span data-ttu-id="c1755-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1755-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1755-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1755-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1755-112">"DelegatedPermissionGrant"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="c1755-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1755-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1755-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1755-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1755-114">Not supported.</span></span>    |
|<span data-ttu-id="c1755-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1755-115">Application</span></span> | <span data-ttu-id="c1755-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1755-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1755-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1755-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1755-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1755-118">Optional query parameters</span></span>

<span data-ttu-id="c1755-119">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1755-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1755-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1755-120">Request headers</span></span>

| <span data-ttu-id="c1755-121">名称</span><span class="sxs-lookup"><span data-stu-id="c1755-121">Name</span></span> | <span data-ttu-id="c1755-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1755-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="c1755-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1755-123">Authorization</span></span>  | <span data-ttu-id="c1755-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c1755-124">Bearer {token}.</span></span> <span data-ttu-id="c1755-125">Required.</span><span class="sxs-lookup"><span data-stu-id="c1755-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1755-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1755-126">Request body</span></span>

<span data-ttu-id="c1755-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1755-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1755-128">响应</span><span class="sxs-lookup"><span data-stu-id="c1755-128">Response</span></span>

<span data-ttu-id="c1755-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1755-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1755-130">示例</span><span class="sxs-lookup"><span data-stu-id="c1755-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1755-131">请求</span><span class="sxs-lookup"><span data-stu-id="c1755-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c1755-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1755-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="c1755-133">C#</span><span class="sxs-lookup"><span data-stu-id="c1755-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1755-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1755-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1755-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1755-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1755-136">响应</span><span class="sxs-lookup"><span data-stu-id="c1755-136">Response</span></span>

> <span data-ttu-id="c1755-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="c1755-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c1755-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c1755-138">All the properties will be returned from an actual call.</span></span>

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
