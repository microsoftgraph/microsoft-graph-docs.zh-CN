---
title: 列表组可传递成员
description: 获取组成员的列表。 组可以将用户、设备、组织联系人和其他组作为成员。 此操作是可传递的，并返回所有嵌套成员的简单列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 99a4abafb5cb879f2f8b7f721a237495055bcde7
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125132"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="cd865-105">列表组可传递成员</span><span class="sxs-lookup"><span data-stu-id="cd865-105">List group transitive members</span></span>

<span data-ttu-id="cd865-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd865-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd865-107">获取组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="cd865-107">Get a list of the group's members.</span></span> <span data-ttu-id="cd865-108">组可以将用户、设备、组织联系人和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="cd865-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="cd865-109">此操作是可传递的，并返回所有嵌套成员的简单列表。</span><span class="sxs-lookup"><span data-stu-id="cd865-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd865-110">权限</span><span class="sxs-lookup"><span data-stu-id="cd865-110">Permissions</span></span>

<span data-ttu-id="cd865-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd865-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd865-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd865-113">Permission type</span></span>      | <span data-ttu-id="cd865-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd865-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd865-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd865-115">Delegated (work or school account)</span></span> | <span data-ttu-id="cd865-116">Directory.accessasuser.all、User.readbasic.all、用户、全部、用户、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="cd865-116">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="cd865-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd865-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd865-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd865-118">Not supported.</span></span>    |
|<span data-ttu-id="cd865-119">Application</span><span class="sxs-lookup"><span data-stu-id="cd865-119">Application</span></span> | <span data-ttu-id="cd865-120">Read. All，User. All</span><span class="sxs-lookup"><span data-stu-id="cd865-120">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="cd865-121">**注意：** 若要列出隐藏的成员资格组的成员，则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="cd865-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="cd865-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd865-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd865-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cd865-123">Optional query parameters</span></span>

<span data-ttu-id="cd865-124">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cd865-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd865-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd865-125">Request headers</span></span>

| <span data-ttu-id="cd865-126">标头</span><span class="sxs-lookup"><span data-stu-id="cd865-126">Header</span></span>       | <span data-ttu-id="cd865-127">值</span><span class="sxs-lookup"><span data-stu-id="cd865-127">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="cd865-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd865-128">Authorization</span></span>  | <span data-ttu-id="cd865-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd865-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd865-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd865-131">Request body</span></span>

<span data-ttu-id="cd865-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd865-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd865-133">响应</span><span class="sxs-lookup"><span data-stu-id="cd865-133">Response</span></span>

<span data-ttu-id="cd865-134">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cd865-134">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd865-135">示例</span><span class="sxs-lookup"><span data-stu-id="cd865-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd865-136">请求</span><span class="sxs-lookup"><span data-stu-id="cd865-136">Request</span></span>

<span data-ttu-id="cd865-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cd865-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd865-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd865-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="cd865-139">C#</span><span class="sxs-lookup"><span data-stu-id="cd865-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd865-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd865-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd865-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd865-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd865-142">Java</span><span class="sxs-lookup"><span data-stu-id="cd865-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd865-143">响应</span><span class="sxs-lookup"><span data-stu-id="cd865-143">Response</span></span>

<span data-ttu-id="cd865-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cd865-144">The following is an example of the response.</span></span>
><span data-ttu-id="cd865-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd865-145">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
