---
title: 列表组可传递成员
description: 获取组成员的列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9116569521cb024cd6501e448f8dccad61f64260
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396815"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="16905-103">列表组可传递成员</span><span class="sxs-lookup"><span data-stu-id="16905-103">List group transitive members</span></span>

<span data-ttu-id="16905-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16905-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16905-105">获取组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="16905-105">Get a list of the group's members.</span></span> <span data-ttu-id="16905-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="16905-106">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="16905-107">此操作是可传递的，并且还将返回所有嵌套成员的简单列表。</span><span class="sxs-lookup"><span data-stu-id="16905-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="16905-108">权限</span><span class="sxs-lookup"><span data-stu-id="16905-108">Permissions</span></span>

<span data-ttu-id="16905-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16905-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16905-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16905-111">Permission type</span></span>      | <span data-ttu-id="16905-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16905-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16905-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16905-113">Delegated (work or school account)</span></span> | <span data-ttu-id="16905-114">Directory.accessasuser.all、User.readbasic.all、用户、全部、用户、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="16905-114">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="16905-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16905-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16905-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16905-116">Not supported.</span></span>    |
|<span data-ttu-id="16905-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16905-117">Application</span></span> | <span data-ttu-id="16905-118">Read. All，User. All</span><span class="sxs-lookup"><span data-stu-id="16905-118">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="16905-119">注意：若要列出隐藏的成员资格组的成员，则需要使用 Read。隐藏权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="16905-119">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="16905-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16905-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16905-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16905-121">Optional query parameters</span></span>

<span data-ttu-id="16905-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16905-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16905-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="16905-123">Request headers</span></span>

| <span data-ttu-id="16905-124">名称</span><span class="sxs-lookup"><span data-stu-id="16905-124">Name</span></span>       | <span data-ttu-id="16905-125">类型</span><span class="sxs-lookup"><span data-stu-id="16905-125">Type</span></span> | <span data-ttu-id="16905-126">说明</span><span class="sxs-lookup"><span data-stu-id="16905-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="16905-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="16905-127">Authorization</span></span>  | <span data-ttu-id="16905-128">string</span><span class="sxs-lookup"><span data-stu-id="16905-128">string</span></span>  | <span data-ttu-id="16905-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16905-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16905-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="16905-131">Request body</span></span>

<span data-ttu-id="16905-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16905-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16905-133">响应</span><span class="sxs-lookup"><span data-stu-id="16905-133">Response</span></span>

<span data-ttu-id="16905-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="16905-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16905-135">示例</span><span class="sxs-lookup"><span data-stu-id="16905-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="16905-136">请求</span><span class="sxs-lookup"><span data-stu-id="16905-136">Request</span></span>

<span data-ttu-id="16905-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16905-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16905-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="16905-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="16905-139">C#</span><span class="sxs-lookup"><span data-stu-id="16905-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16905-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16905-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16905-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16905-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16905-142">响应</span><span class="sxs-lookup"><span data-stu-id="16905-142">Response</span></span>

<span data-ttu-id="16905-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16905-143">The following is an example of the response.</span></span>
><span data-ttu-id="16905-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16905-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16905-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="16905-145">All the properties will be returned from an actual call.</span></span>
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
