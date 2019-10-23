---
title: 列出 transitiveMemberOf
description: 获取 organziational 联系人所属的组。 此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 97f787dad12e499b64d43714e3cbe7b27be36d39
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633902"
---
# <a name="list-transitivememberof"></a><span data-ttu-id="80cb6-104">列出 transitiveMemberOf</span><span class="sxs-lookup"><span data-stu-id="80cb6-104">List transitiveMemberOf</span></span>

<span data-ttu-id="80cb6-105">获取此[组织联系人](../resources/orgcontact.md)所属的组。</span><span class="sxs-lookup"><span data-stu-id="80cb6-105">Get groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="80cb6-106">API 请求是可传递的，并返回组织联系人是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="80cb6-106">The API request is transitive, and returns all groups the organizational contact is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="80cb6-107">权限</span><span class="sxs-lookup"><span data-stu-id="80cb6-107">Permissions</span></span>

<span data-ttu-id="80cb6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80cb6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80cb6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="80cb6-110">Permission type</span></span>      | <span data-ttu-id="80cb6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80cb6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80cb6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80cb6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="80cb6-113">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="80cb6-113">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="80cb6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80cb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80cb6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80cb6-115">Not supported.</span></span>    |
|<span data-ttu-id="80cb6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="80cb6-116">Application</span></span> | <span data-ttu-id="80cb6-117">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="80cb6-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80cb6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80cb6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80cb6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80cb6-119">Optional query parameters</span></span>

<span data-ttu-id="80cb6-120">此方法支持`$select` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80cb6-120">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80cb6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="80cb6-121">Request headers</span></span>

| <span data-ttu-id="80cb6-122">标头</span><span class="sxs-lookup"><span data-stu-id="80cb6-122">Header</span></span>       | <span data-ttu-id="80cb6-123">值</span><span class="sxs-lookup"><span data-stu-id="80cb6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80cb6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="80cb6-124">Authorization</span></span>  | <span data-ttu-id="80cb6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80cb6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="80cb6-127">接受</span><span class="sxs-lookup"><span data-stu-id="80cb6-127">Accept</span></span>  | <span data-ttu-id="80cb6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="80cb6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80cb6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="80cb6-129">Request body</span></span>

<span data-ttu-id="80cb6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80cb6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80cb6-131">响应</span><span class="sxs-lookup"><span data-stu-id="80cb6-131">Response</span></span>

<span data-ttu-id="80cb6-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="80cb6-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80cb6-133">示例</span><span class="sxs-lookup"><span data-stu-id="80cb6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="80cb6-134">请求</span><span class="sxs-lookup"><span data-stu-id="80cb6-134">Request</span></span>

<span data-ttu-id="80cb6-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80cb6-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80cb6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="80cb6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_list_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80cb6-137">C#</span><span class="sxs-lookup"><span data-stu-id="80cb6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-list-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80cb6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80cb6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-list-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80cb6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80cb6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-list-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="80cb6-140">Java</span><span class="sxs-lookup"><span data-stu-id="80cb6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-list-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80cb6-141">响应</span><span class="sxs-lookup"><span data-stu-id="80cb6-141">Response</span></span>

<span data-ttu-id="80cb6-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="80cb6-142">The following is an example of the response.</span></span>
><span data-ttu-id="80cb6-143">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80cb6-143">**Note**: The response object shown here might be shortened for readability.</span></span> 

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
