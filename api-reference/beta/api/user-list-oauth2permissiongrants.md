---
title: List oauth2PermissionGrants
description: 检索 oAuth2PermissionGrant 对象的列表，表示委派的权限授予。
localization_priority: Priority
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: b2bab33e8e78c7c42e7d47fd6dcf4a889579528b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231789"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="afb15-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="afb15-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="afb15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afb15-105">检索 [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) 实体的列表，表示授予以使客户端应用程序能够代表用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="afb15-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="afb15-106">查询对用户的委派权限授予将仅返回特定于给定用户的委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="afb15-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="afb15-107">代表组织中所有用户授予的委派权限 _未_ 包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="afb15-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

> [!NOTE]
> <span data-ttu-id="afb15-108">此请求对最近创建、更新或删除的委派权限授予可能具有复制延迟。</span><span class="sxs-lookup"><span data-stu-id="afb15-108">This request might have replication delays for delegated permission grants that were recently created, updated, or deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="afb15-109">权限</span><span class="sxs-lookup"><span data-stu-id="afb15-109">Permissions</span></span>

<span data-ttu-id="afb15-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afb15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb15-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="afb15-112">Permission type</span></span>      | <span data-ttu-id="afb15-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afb15-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afb15-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afb15-114">Delegated (work or school account)</span></span> | <span data-ttu-id="afb15-115">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afb15-115">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="afb15-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afb15-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb15-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="afb15-117">Not supported.</span></span>    |
|<span data-ttu-id="afb15-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="afb15-118">Application</span></span> | <span data-ttu-id="afb15-119">.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb15-119">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afb15-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afb15-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afb15-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="afb15-121">Optional query parameters</span></span>

<span data-ttu-id="afb15-122">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="afb15-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afb15-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="afb15-123">Request headers</span></span>

| <span data-ttu-id="afb15-124">名称</span><span class="sxs-lookup"><span data-stu-id="afb15-124">Name</span></span>           | <span data-ttu-id="afb15-125">说明</span><span class="sxs-lookup"><span data-stu-id="afb15-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="afb15-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="afb15-126">Authorization</span></span>  | <span data-ttu-id="afb15-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="afb15-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="afb15-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="afb15-129">Request body</span></span>

<span data-ttu-id="afb15-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="afb15-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afb15-131">响应</span><span class="sxs-lookup"><span data-stu-id="afb15-131">Response</span></span>

<span data-ttu-id="afb15-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="afb15-132">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afb15-133">示例</span><span class="sxs-lookup"><span data-stu-id="afb15-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afb15-134">请求</span><span class="sxs-lookup"><span data-stu-id="afb15-134">Request</span></span>

<span data-ttu-id="afb15-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afb15-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="afb15-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="afb15-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="afb15-137">C#</span><span class="sxs-lookup"><span data-stu-id="afb15-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afb15-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afb15-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afb15-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afb15-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afb15-140">Java</span><span class="sxs-lookup"><span data-stu-id="afb15-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="afb15-141">响应</span><span class="sxs-lookup"><span data-stu-id="afb15-141">Response</span></span>

<span data-ttu-id="afb15-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="afb15-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="afb15-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="afb15-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "clientId": "85477313-ea43-4c7d-b8a4-54fed35d0b60",
      "consentType": "Principal",
      "expiryTime": "2021-09-19T07:06:52.6843299Z",
      "id": "E3NHhUPqfUy4pFT-010LYFo5-ycA-_5Fhl7nHbaJ7qACy1R9o6oWQJ-cpLSUIt2b",
      "principalId": "7d54cb02-aaa3-4016-9f9c-a4b49422dd9b",
      "resourceId": "27fb395a-fb00-45fe-865e-e71db689eea0",
      "scope": " Contacts.ReadWrite openid profile",
      "startTime": "0001-01-01T00:00:00Z"
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


