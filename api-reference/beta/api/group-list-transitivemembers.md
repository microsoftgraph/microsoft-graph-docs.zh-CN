---
title: 列表组可传递成员
description: 获取组成员的列表。 组可以将用户、联系人、设备、服务主体和其他组作为成员。 此操作是可传递的，并且还将返回所有嵌套成员的简单列表。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5ff85a96025a605671fa0cd64a7d68c2f67ead7e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869603"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="a1c88-105">列表组可传递成员</span><span class="sxs-lookup"><span data-stu-id="a1c88-105">List group transitive members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1c88-106">获取组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="a1c88-106">Get a list of the group's members.</span></span> <span data-ttu-id="a1c88-107">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="a1c88-107">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="a1c88-108">此操作是可传递的，并且还将返回所有嵌套成员的简单列表。</span><span class="sxs-lookup"><span data-stu-id="a1c88-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1c88-109">权限</span><span class="sxs-lookup"><span data-stu-id="a1c88-109">Permissions</span></span>

<span data-ttu-id="a1c88-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1c88-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1c88-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1c88-112">Permission type</span></span>      | <span data-ttu-id="a1c88-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1c88-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1c88-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1c88-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a1c88-115">Directory.accessasuser.all、User.readbasic.all、用户、全部、用户、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="a1c88-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="a1c88-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1c88-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1c88-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1c88-117">Not supported.</span></span>    |
|<span data-ttu-id="a1c88-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1c88-118">Application</span></span> | <span data-ttu-id="a1c88-119">Read. All，User. All</span><span class="sxs-lookup"><span data-stu-id="a1c88-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="a1c88-120">注意：若要列出隐藏的成员资格组的成员，则需要使用 Read。隐藏权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="a1c88-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a1c88-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1c88-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1c88-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1c88-122">Optional query parameters</span></span>

<span data-ttu-id="a1c88-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a1c88-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1c88-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1c88-124">Request headers</span></span>

| <span data-ttu-id="a1c88-125">名称</span><span class="sxs-lookup"><span data-stu-id="a1c88-125">Name</span></span>       | <span data-ttu-id="a1c88-126">类型</span><span class="sxs-lookup"><span data-stu-id="a1c88-126">Type</span></span> | <span data-ttu-id="a1c88-127">说明</span><span class="sxs-lookup"><span data-stu-id="a1c88-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1c88-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1c88-128">Authorization</span></span>  | <span data-ttu-id="a1c88-129">string</span><span class="sxs-lookup"><span data-stu-id="a1c88-129">string</span></span>  | <span data-ttu-id="a1c88-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1c88-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1c88-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1c88-132">Request body</span></span>

<span data-ttu-id="a1c88-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1c88-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1c88-134">响应</span><span class="sxs-lookup"><span data-stu-id="a1c88-134">Response</span></span>

<span data-ttu-id="a1c88-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a1c88-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1c88-136">示例</span><span class="sxs-lookup"><span data-stu-id="a1c88-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1c88-137">请求</span><span class="sxs-lookup"><span data-stu-id="a1c88-137">Request</span></span>

<span data-ttu-id="a1c88-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1c88-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a1c88-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c88-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1c88-140">C#</span><span class="sxs-lookup"><span data-stu-id="a1c88-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1c88-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1c88-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1c88-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1c88-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1c88-143">响应</span><span class="sxs-lookup"><span data-stu-id="a1c88-143">Response</span></span>

<span data-ttu-id="a1c88-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a1c88-144">The following is an example of the response.</span></span>
><span data-ttu-id="a1c88-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a1c88-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a1c88-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a1c88-146">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
