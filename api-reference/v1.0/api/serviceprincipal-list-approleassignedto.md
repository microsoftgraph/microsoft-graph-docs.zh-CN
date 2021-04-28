---
title: 列出为服务主体授予的 appRoleAssignment
description: 检索为服务主体授予的应用角色分配列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 9a9cfd5330d21fe8e8199c9a7fec58c8bb470e7d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049427"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="fdd7e-103">列出为服务主体授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fdd7e-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="fdd7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdd7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fdd7e-105">检索已为给定资源服务主体授予用户、组或客户端服务主体的 [appRoleAssignment ](../resources/approleassignment.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="fdd7e-106">例如，如果资源服务主体是 Microsoft Graph API 的服务主体，则将返回已向 Microsoft Graph 授予任何仅应用权限的所有服务主体。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="fdd7e-107">如果资源服务主体是具有授予用户和组的应用角色的应用程序，则将返回为此应用程序分配应用角色的所有用户和组。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdd7e-108">权限</span><span class="sxs-lookup"><span data-stu-id="fdd7e-108">Permissions</span></span>

<span data-ttu-id="fdd7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdd7e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdd7e-111">Permission type</span></span>      | <span data-ttu-id="fdd7e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fdd7e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdd7e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdd7e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fdd7e-114">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fdd7e-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="fdd7e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdd7e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdd7e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-116">Not supported.</span></span>    |
|<span data-ttu-id="fdd7e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdd7e-117">Application</span></span> | <span data-ttu-id="fdd7e-118">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd7e-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdd7e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdd7e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdd7e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fdd7e-120">Optional query parameters</span></span>

<span data-ttu-id="fdd7e-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdd7e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdd7e-122">Request headers</span></span>

| <span data-ttu-id="fdd7e-123">名称</span><span class="sxs-lookup"><span data-stu-id="fdd7e-123">Name</span></span>           | <span data-ttu-id="fdd7e-124">说明</span><span class="sxs-lookup"><span data-stu-id="fdd7e-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="fdd7e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdd7e-125">Authorization</span></span>  | <span data-ttu-id="fdd7e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fdd7e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdd7e-128">Request body</span></span>

<span data-ttu-id="fdd7e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdd7e-130">响应</span><span class="sxs-lookup"><span data-stu-id="fdd7e-130">Response</span></span>

<span data-ttu-id="fdd7e-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdd7e-132">示例</span><span class="sxs-lookup"><span data-stu-id="fdd7e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdd7e-133">请求</span><span class="sxs-lookup"><span data-stu-id="fdd7e-133">Request</span></span>

<span data-ttu-id="fdd7e-134">以下是检索已为给定资源服务主体授予的应用角色分配的请求示例。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="fdd7e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdd7e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo
```
# <a name="c"></a>[<span data-ttu-id="fdd7e-136">C#</span><span class="sxs-lookup"><span data-stu-id="fdd7e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdd7e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdd7e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdd7e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdd7e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdd7e-139">Java</span><span class="sxs-lookup"><span data-stu-id="fdd7e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fdd7e-140">响应</span><span class="sxs-lookup"><span data-stu-id="fdd7e-140">Response</span></span>

<span data-ttu-id="fdd7e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="fdd7e-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fdd7e-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('8e881353-1735-45af-af21-ee1344582a4d')/appRoleAssignedTo",
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "createdDateTime": "2021-02-02T04:22:45.9480566Z",
      "principalDisplayName": "MOD Administrator",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
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

