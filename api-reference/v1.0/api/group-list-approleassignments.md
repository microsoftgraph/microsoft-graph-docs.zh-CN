---
title: 列出向组授予的 appRoleAssignment
description: 检索已授予组的 appRoleAssignments 列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: 90c8b025b739722b927e9b2f0ac63d6bca51294e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052346"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="7809c-103">列出向组授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7809c-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="7809c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7809c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7809c-105">检索已授予组的 [appRoleAssignment](../resources/approleassignment.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="7809c-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="7809c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7809c-106">Permissions</span></span>

<span data-ttu-id="7809c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7809c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7809c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7809c-109">Permission type</span></span>      | <span data-ttu-id="7809c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7809c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7809c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7809c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7809c-112">Directory.Read.All、AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7809c-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="7809c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7809c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7809c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7809c-114">Not supported.</span></span>    |
|<span data-ttu-id="7809c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7809c-115">Application</span></span> | <span data-ttu-id="7809c-116">Directory.Read.All、AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7809c-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7809c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7809c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7809c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7809c-118">Optional query parameters</span></span>

<span data-ttu-id="7809c-119">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7809c-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7809c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7809c-120">Request headers</span></span>

| <span data-ttu-id="7809c-121">名称</span><span class="sxs-lookup"><span data-stu-id="7809c-121">Name</span></span>           | <span data-ttu-id="7809c-122">说明</span><span class="sxs-lookup"><span data-stu-id="7809c-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="7809c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7809c-123">Authorization</span></span>  | <span data-ttu-id="7809c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7809c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7809c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7809c-126">Request body</span></span>

<span data-ttu-id="7809c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7809c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7809c-128">响应</span><span class="sxs-lookup"><span data-stu-id="7809c-128">Response</span></span>

<span data-ttu-id="7809c-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7809c-129">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7809c-130">示例</span><span class="sxs-lookup"><span data-stu-id="7809c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7809c-131">请求</span><span class="sxs-lookup"><span data-stu-id="7809c-131">Request</span></span>

<span data-ttu-id="7809c-132">以下示例显示了检索已分配给组的应用角色的请求。</span><span class="sxs-lookup"><span data-stu-id="7809c-132">The following example shows a request to retrieve the app roles that have been assigned to a group.</span></span>


# <a name="http"></a>[<span data-ttu-id="7809c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7809c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="7809c-134">C#</span><span class="sxs-lookup"><span data-stu-id="7809c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7809c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7809c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7809c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7809c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7809c-137">Java</span><span class="sxs-lookup"><span data-stu-id="7809c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7809c-138">响应</span><span class="sxs-lookup"><span data-stu-id="7809c-138">Response</span></span>

<span data-ttu-id="7809c-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7809c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="7809c-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7809c-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments",
  "value": [
    {
      "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "createdDateTime": "2021-02-19T17:55:08.3369542Z",
      "principalDisplayName": "Young techmakers",
      "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
      "principalType": "Group",
      "resourceDisplayName": "Yammer",
      "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

