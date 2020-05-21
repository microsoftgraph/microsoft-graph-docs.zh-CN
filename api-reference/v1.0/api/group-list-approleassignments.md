---
title: 向组授予的列表 appRoleAssignments
description: 检索已授予组的 appRoleAssignments 的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 947271309c2e6aabc1dcce0760770eb3f2df7c12
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336540"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="9be53-103">向组授予的列表 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="9be53-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="9be53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9be53-105">检索已授予组的[appRoleAssignment](../resources/approleassignment.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="9be53-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="9be53-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9be53-106">Permissions</span></span>

<span data-ttu-id="9be53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9be53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9be53-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9be53-109">Permission type</span></span>      | <span data-ttu-id="9be53-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9be53-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9be53-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9be53-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9be53-112">"AppRoleAssignment"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="9be53-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="9be53-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9be53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be53-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9be53-114">Not supported.</span></span>    |
|<span data-ttu-id="9be53-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9be53-115">Application</span></span> | <span data-ttu-id="9be53-116">"AppRoleAssignment"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="9be53-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9be53-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9be53-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9be53-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9be53-118">Optional query parameters</span></span>

<span data-ttu-id="9be53-119">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9be53-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9be53-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9be53-120">Request headers</span></span>

| <span data-ttu-id="9be53-121">名称</span><span class="sxs-lookup"><span data-stu-id="9be53-121">Name</span></span>           | <span data-ttu-id="9be53-122">说明</span><span class="sxs-lookup"><span data-stu-id="9be53-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="9be53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9be53-123">Authorization</span></span>  | <span data-ttu-id="9be53-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9be53-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9be53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9be53-126">Request body</span></span>

<span data-ttu-id="9be53-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9be53-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9be53-128">响应</span><span class="sxs-lookup"><span data-stu-id="9be53-128">Response</span></span>

<span data-ttu-id="9be53-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9be53-129">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9be53-130">示例</span><span class="sxs-lookup"><span data-stu-id="9be53-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9be53-131">请求</span><span class="sxs-lookup"><span data-stu-id="9be53-131">Request</span></span>

<span data-ttu-id="9be53-132">下面的示例演示了一个检索已分配给组的应用程序角色的请求。</span><span class="sxs-lookup"><span data-stu-id="9be53-132">The following example shows a request to retrieve the app roles that have been assigned to a group.</span></span>


# <a name="http"></a>[<span data-ttu-id="9be53-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9be53-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="9be53-134">C#</span><span class="sxs-lookup"><span data-stu-id="9be53-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9be53-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9be53-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9be53-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9be53-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9be53-137">Java</span><span class="sxs-lookup"><span data-stu-id="9be53-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9be53-138">响应</span><span class="sxs-lookup"><span data-stu-id="9be53-138">Response</span></span>

<span data-ttu-id="9be53-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9be53-139">The following is an example of the response.</span></span>

> <span data-ttu-id="9be53-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9be53-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
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
