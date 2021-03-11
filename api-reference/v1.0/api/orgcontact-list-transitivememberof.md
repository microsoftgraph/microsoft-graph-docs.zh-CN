---
title: 列出 transitiveMemberOf
description: 获取组织联系人是其中一个成员的组。 此 API 请求是可传递的，并且还将返回用户是嵌套成员的所有组。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 94a41d23225615a6233b8d37a5cded8f569c7898
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625988"
---
# <a name="list-transitivememberof"></a><span data-ttu-id="48878-104">列出 transitiveMemberOf</span><span class="sxs-lookup"><span data-stu-id="48878-104">List transitiveMemberOf</span></span>

<span data-ttu-id="48878-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48878-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48878-106">获取此 [组织联系人是](../resources/orgcontact.md) 其中一个成员的组。</span><span class="sxs-lookup"><span data-stu-id="48878-106">Get groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="48878-107">API 请求是可传递的，并返回组织联系人是嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="48878-107">The API request is transitive, and returns all groups the organizational contact is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="48878-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="48878-108">Permissions</span></span>

<span data-ttu-id="48878-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48878-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48878-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48878-111">Permission type</span></span>      | <span data-ttu-id="48878-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48878-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48878-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48878-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48878-114">OrgContact.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="48878-114">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="48878-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48878-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48878-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48878-116">Not supported.</span></span>    |
|<span data-ttu-id="48878-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48878-117">Application</span></span> | <span data-ttu-id="48878-118">OrgContact.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="48878-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48878-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48878-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48878-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="48878-120">Optional query parameters</span></span>

<span data-ttu-id="48878-121">此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="48878-121">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48878-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="48878-122">Request headers</span></span>

| <span data-ttu-id="48878-123">标头</span><span class="sxs-lookup"><span data-stu-id="48878-123">Header</span></span>       | <span data-ttu-id="48878-124">值</span><span class="sxs-lookup"><span data-stu-id="48878-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48878-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="48878-125">Authorization</span></span>  | <span data-ttu-id="48878-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48878-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48878-128">接受</span><span class="sxs-lookup"><span data-stu-id="48878-128">Accept</span></span>  | <span data-ttu-id="48878-129">application/json</span><span class="sxs-lookup"><span data-stu-id="48878-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48878-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="48878-130">Request body</span></span>

<span data-ttu-id="48878-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48878-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48878-132">响应</span><span class="sxs-lookup"><span data-stu-id="48878-132">Response</span></span>

<span data-ttu-id="48878-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="48878-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48878-134">示例</span><span class="sxs-lookup"><span data-stu-id="48878-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="48878-135">请求</span><span class="sxs-lookup"><span data-stu-id="48878-135">Request</span></span>

<span data-ttu-id="48878-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48878-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "orgcontact_list_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="48878-137">响应</span><span class="sxs-lookup"><span data-stu-id="48878-137">Response</span></span>

<span data-ttu-id="48878-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48878-138">The following is an example of the response.</span></span>
><span data-ttu-id="48878-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="48878-139">**Note**: The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

