---
title: List oauth2PermissionGrants
description: 检索 oAuth2PermissionGrant 对象的列表，表示委派的权限授予。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: aba0f22c3eda597309a2af0079a1e1f7aa99cf24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992130"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="36c0b-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="36c0b-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="36c0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36c0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36c0b-105">检索 [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) 实体的列表，表示授予以使客户端应用程序能够代表用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="36c0b-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="36c0b-106">查询对用户的委派权限授予将仅返回特定于给定用户的委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="36c0b-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="36c0b-107">代表组织中所有用户授予的委派权限_未_包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="36c0b-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="36c0b-108">权限</span><span class="sxs-lookup"><span data-stu-id="36c0b-108">Permissions</span></span>

<span data-ttu-id="36c0b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36c0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c0b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36c0b-111">Permission type</span></span>      | <span data-ttu-id="36c0b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36c0b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36c0b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36c0b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="36c0b-114">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36c0b-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="36c0b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36c0b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36c0b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36c0b-116">Not supported.</span></span>    |
|<span data-ttu-id="36c0b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36c0b-117">Application</span></span> | <span data-ttu-id="36c0b-118">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c0b-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36c0b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36c0b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36c0b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36c0b-120">Optional query parameters</span></span>

<span data-ttu-id="36c0b-121">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="36c0b-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36c0b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="36c0b-122">Request headers</span></span>

| <span data-ttu-id="36c0b-123">名称</span><span class="sxs-lookup"><span data-stu-id="36c0b-123">Name</span></span>           | <span data-ttu-id="36c0b-124">说明</span><span class="sxs-lookup"><span data-stu-id="36c0b-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="36c0b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c0b-125">Authorization</span></span>  | <span data-ttu-id="36c0b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36c0b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36c0b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="36c0b-128">Request body</span></span>

<span data-ttu-id="36c0b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36c0b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36c0b-130">响应</span><span class="sxs-lookup"><span data-stu-id="36c0b-130">Response</span></span>

<span data-ttu-id="36c0b-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="36c0b-131">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36c0b-132">示例</span><span class="sxs-lookup"><span data-stu-id="36c0b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36c0b-133">请求</span><span class="sxs-lookup"><span data-stu-id="36c0b-133">Request</span></span>

<span data-ttu-id="36c0b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36c0b-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36c0b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="36c0b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="36c0b-136">C#</span><span class="sxs-lookup"><span data-stu-id="36c0b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36c0b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36c0b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36c0b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36c0b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36c0b-139">Java</span><span class="sxs-lookup"><span data-stu-id="36c0b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36c0b-140">响应</span><span class="sxs-lookup"><span data-stu-id="36c0b-140">Response</span></span>

<span data-ttu-id="36c0b-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="36c0b-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="36c0b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="36c0b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 253

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

