---
title: 列出 transitiveMemberOf
description: 获取 organziational 联系人所属的组。 此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 780abea12cf61655f8d529dadf2f8c4414401dc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032899"
---
# <a name="list-transitivememberof"></a><span data-ttu-id="16531-104">列出 transitiveMemberOf</span><span class="sxs-lookup"><span data-stu-id="16531-104">List transitiveMemberOf</span></span>

<span data-ttu-id="16531-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16531-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16531-106">获取此 [组织联系人](../resources/orgcontact.md) 所属的组。</span><span class="sxs-lookup"><span data-stu-id="16531-106">Get groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="16531-107">API 请求是可传递的，并返回组织联系人是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="16531-107">The API request is transitive, and returns all groups the organizational contact is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="16531-108">权限</span><span class="sxs-lookup"><span data-stu-id="16531-108">Permissions</span></span>

<span data-ttu-id="16531-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16531-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16531-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16531-111">Permission type</span></span>      | <span data-ttu-id="16531-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16531-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16531-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16531-113">Delegated (work or school account)</span></span> | <span data-ttu-id="16531-114">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="16531-114">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="16531-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16531-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16531-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16531-116">Not supported.</span></span>    |
|<span data-ttu-id="16531-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16531-117">Application</span></span> | <span data-ttu-id="16531-118">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="16531-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16531-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16531-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16531-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16531-120">Optional query parameters</span></span>

<span data-ttu-id="16531-121">此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16531-121">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16531-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="16531-122">Request headers</span></span>

| <span data-ttu-id="16531-123">标头</span><span class="sxs-lookup"><span data-stu-id="16531-123">Header</span></span>       | <span data-ttu-id="16531-124">值</span><span class="sxs-lookup"><span data-stu-id="16531-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16531-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16531-125">Authorization</span></span>  | <span data-ttu-id="16531-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16531-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16531-128">接受</span><span class="sxs-lookup"><span data-stu-id="16531-128">Accept</span></span>  | <span data-ttu-id="16531-129">application/json</span><span class="sxs-lookup"><span data-stu-id="16531-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16531-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="16531-130">Request body</span></span>

<span data-ttu-id="16531-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16531-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16531-132">响应</span><span class="sxs-lookup"><span data-stu-id="16531-132">Response</span></span>

<span data-ttu-id="16531-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="16531-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16531-134">示例</span><span class="sxs-lookup"><span data-stu-id="16531-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="16531-135">请求</span><span class="sxs-lookup"><span data-stu-id="16531-135">Request</span></span>

<span data-ttu-id="16531-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16531-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16531-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="16531-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_list_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="16531-138">C#</span><span class="sxs-lookup"><span data-stu-id="16531-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-list-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16531-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16531-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-list-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16531-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16531-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-list-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16531-141">Java</span><span class="sxs-lookup"><span data-stu-id="16531-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-list-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16531-142">响应</span><span class="sxs-lookup"><span data-stu-id="16531-142">Response</span></span>

<span data-ttu-id="16531-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16531-143">The following is an example of the response.</span></span>
><span data-ttu-id="16531-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16531-144">**Note**: The response object shown here might be shortened for readability.</span></span> 

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

