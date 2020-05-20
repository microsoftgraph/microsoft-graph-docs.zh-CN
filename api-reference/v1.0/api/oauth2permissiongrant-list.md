---
title: 列出 oAuth2PermissionGrants
description: 检索 oauth2PermissionGrant 对象的列表，表示委派权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 49c15d70947d991b6bb9b326d148836557ef8f93
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288705"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="dc888-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="dc888-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="dc888-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc888-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc888-105">检索[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象的列表，这些对象代表已为客户端应用程序授予的代表登录用户访问 api 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="dc888-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc888-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dc888-106">Permissions</span></span>

<span data-ttu-id="dc888-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc888-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc888-109">Permission type</span></span>      | <span data-ttu-id="dc888-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc888-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc888-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc888-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc888-112">"DelegatedPermissionGrant"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="dc888-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc888-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc888-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc888-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc888-114">Not supported.</span></span>    |
|<span data-ttu-id="dc888-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc888-115">Application</span></span> | <span data-ttu-id="dc888-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc888-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc888-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc888-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc888-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dc888-118">Optional query parameters</span></span>

<span data-ttu-id="dc888-119">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dc888-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc888-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc888-120">Request headers</span></span>

| <span data-ttu-id="dc888-121">名称</span><span class="sxs-lookup"><span data-stu-id="dc888-121">Name</span></span> | <span data-ttu-id="dc888-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc888-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="dc888-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc888-123">Authorization</span></span>  | <span data-ttu-id="dc888-124">string</span><span class="sxs-lookup"><span data-stu-id="dc888-124">string</span></span>  | <span data-ttu-id="dc888-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc888-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc888-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc888-127">Request body</span></span>

<span data-ttu-id="dc888-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc888-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc888-129">响应</span><span class="sxs-lookup"><span data-stu-id="dc888-129">Response</span></span>

<span data-ttu-id="dc888-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="dc888-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc888-131">示例</span><span class="sxs-lookup"><span data-stu-id="dc888-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc888-132">请求</span><span class="sxs-lookup"><span data-stu-id="dc888-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```http
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants
```

### <a name="response"></a><span data-ttu-id="dc888-133">响应</span><span class="sxs-lookup"><span data-stu-id="dc888-133">Response</span></span>

> <span data-ttu-id="dc888-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dc888-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
