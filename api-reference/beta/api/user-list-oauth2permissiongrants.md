---
title: List oauth2PermissionGrants
description: 检索 oAuth2PermissionGrant 对象的列表，表示委派权限授予。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e186cb95f7b25ec77c07fadb6c1d0a3095e03d96
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290663"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="de871-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="de871-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="de871-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de871-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de871-105">检索[oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md)实体的列表，这些实体表示为使客户端应用程序能够代表用户访问 API 而授予的委派权限。</span><span class="sxs-lookup"><span data-stu-id="de871-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="de871-106">查询用户的委派权限授予将仅返回特定用户专用的委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="de871-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="de871-107">在组织中代表所有用户授予的委派权限_不_包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="de871-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="de871-108">权限</span><span class="sxs-lookup"><span data-stu-id="de871-108">Permissions</span></span>

<span data-ttu-id="de871-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de871-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de871-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de871-111">Permission type</span></span>      | <span data-ttu-id="de871-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de871-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de871-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de871-113">Delegated (work or school account)</span></span> | <span data-ttu-id="de871-114">"DelegatedPermissionGrant"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="de871-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="de871-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de871-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de871-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de871-116">Not supported.</span></span>    |
|<span data-ttu-id="de871-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de871-117">Application</span></span> | <span data-ttu-id="de871-118">"DelegatedPermissionGrant"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="de871-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de871-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de871-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de871-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="de871-120">Optional query parameters</span></span>

<span data-ttu-id="de871-121">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="de871-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de871-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="de871-122">Request headers</span></span>

| <span data-ttu-id="de871-123">名称</span><span class="sxs-lookup"><span data-stu-id="de871-123">Name</span></span>           | <span data-ttu-id="de871-124">说明</span><span class="sxs-lookup"><span data-stu-id="de871-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="de871-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="de871-125">Authorization</span></span>  | <span data-ttu-id="de871-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de871-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de871-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="de871-128">Request body</span></span>

<span data-ttu-id="de871-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de871-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de871-130">响应</span><span class="sxs-lookup"><span data-stu-id="de871-130">Response</span></span>

<span data-ttu-id="de871-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="de871-131">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de871-132">示例</span><span class="sxs-lookup"><span data-stu-id="de871-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de871-133">请求</span><span class="sxs-lookup"><span data-stu-id="de871-133">Request</span></span>

<span data-ttu-id="de871-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de871-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/oauth2PermissionGrants
```

### <a name="response"></a><span data-ttu-id="de871-135">响应</span><span class="sxs-lookup"><span data-stu-id="de871-135">Response</span></span>

<span data-ttu-id="de871-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="de871-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="de871-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="de871-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
