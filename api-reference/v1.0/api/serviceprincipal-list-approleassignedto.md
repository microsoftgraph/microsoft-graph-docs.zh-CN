---
title: 为服务主体授予的列表 appRoleAssignments
description: 检索为服务主体授予的应用程序角色分配的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a0339bc03dd6621bc8eb513d91ee4b9b7ac13822
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336236"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="fe87c-103">为服务主体授予的列表 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="fe87c-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="fe87c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe87c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe87c-105">检索已授予给定资源服务主体的用户、组或客户端服务主体的[appRoleAssignment](../resources/approleassignment.md)列表。</span><span class="sxs-lookup"><span data-stu-id="fe87c-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="fe87c-106">例如，如果资源服务主体是 Microsoft Graph API 的服务主体，这将返回所有已向其授予了对 Microsoft Graph 的仅限应用程序权限的服务主体。</span><span class="sxs-lookup"><span data-stu-id="fe87c-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="fe87c-107">如果资源服务主体是向用户和组授予应用程序角色的应用程序，这将返回为此应用程序分配的应用程序角色的所有用户和组。</span><span class="sxs-lookup"><span data-stu-id="fe87c-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe87c-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="fe87c-108">Permissions</span></span>

<span data-ttu-id="fe87c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe87c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe87c-111">Permission type</span></span>      | <span data-ttu-id="fe87c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe87c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe87c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe87c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fe87c-114">"AppRoleAssignment"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="fe87c-114">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="fe87c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe87c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe87c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe87c-116">Not supported.</span></span>    |
|<span data-ttu-id="fe87c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe87c-117">Application</span></span> | <span data-ttu-id="fe87c-118">"AppRoleAssignment"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="fe87c-118">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe87c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe87c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe87c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fe87c-120">Optional query parameters</span></span>

<span data-ttu-id="fe87c-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe87c-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe87c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe87c-122">Request headers</span></span>

| <span data-ttu-id="fe87c-123">名称</span><span class="sxs-lookup"><span data-stu-id="fe87c-123">Name</span></span>           | <span data-ttu-id="fe87c-124">说明</span><span class="sxs-lookup"><span data-stu-id="fe87c-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="fe87c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe87c-125">Authorization</span></span>  | <span data-ttu-id="fe87c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe87c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe87c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe87c-128">Request body</span></span>

<span data-ttu-id="fe87c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe87c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe87c-130">响应</span><span class="sxs-lookup"><span data-stu-id="fe87c-130">Response</span></span>

<span data-ttu-id="fe87c-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe87c-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe87c-132">示例</span><span class="sxs-lookup"><span data-stu-id="fe87c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe87c-133">请求</span><span class="sxs-lookup"><span data-stu-id="fe87c-133">Request</span></span>

<span data-ttu-id="fe87c-134">下面的示例演示了检索已授予给定资源服务主体的应用程序角色分配的请求。</span><span class="sxs-lookup"><span data-stu-id="fe87c-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="fe87c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe87c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignedTo
```
# <a name="c"></a>[<span data-ttu-id="fe87c-136">C#</span><span class="sxs-lookup"><span data-stu-id="fe87c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe87c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe87c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe87c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe87c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe87c-139">Java</span><span class="sxs-lookup"><span data-stu-id="fe87c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe87c-140">响应</span><span class="sxs-lookup"><span data-stu-id="fe87c-140">Response</span></span>

<span data-ttu-id="fe87c-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fe87c-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="fe87c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fe87c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
