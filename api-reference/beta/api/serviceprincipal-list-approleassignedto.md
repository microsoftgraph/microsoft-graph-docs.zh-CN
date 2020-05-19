---
title: 为服务主体授予的列表 appRoleAssignments
description: 检索为服务主体授予的应用程序角色分配的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a30c80bd2dff43db3a505f593c0b30780565eef1
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291235"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="38771-103">为服务主体授予的列表 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="38771-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="38771-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38771-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38771-105">检索已授予给定资源服务主体的用户、组或客户端服务主体的[appRoleAssignment](../resources/approleassignment.md)列表。</span><span class="sxs-lookup"><span data-stu-id="38771-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="38771-106">例如，如果资源服务主体是 Microsoft Graph API 的服务主体，这将返回所有已向其授予了对 Microsoft Graph 的仅限应用程序权限的服务主体。</span><span class="sxs-lookup"><span data-stu-id="38771-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="38771-107">如果资源服务主体是向用户和组授予应用程序角色的应用程序，这将返回为此应用程序分配的应用程序角色的所有用户和组。</span><span class="sxs-lookup"><span data-stu-id="38771-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="38771-108">权限</span><span class="sxs-lookup"><span data-stu-id="38771-108">Permissions</span></span>

<span data-ttu-id="38771-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38771-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38771-111">Permission type</span></span>      | <span data-ttu-id="38771-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38771-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38771-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38771-113">Delegated (work or school account)</span></span> | <span data-ttu-id="38771-114">"AppRoleAssignment"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="38771-114">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="38771-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38771-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38771-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38771-116">Not supported.</span></span>    |
|<span data-ttu-id="38771-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="38771-117">Application</span></span> | <span data-ttu-id="38771-118">"AppRoleAssignment"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="38771-118">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38771-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38771-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38771-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="38771-120">Optional query parameters</span></span>

<span data-ttu-id="38771-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="38771-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38771-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="38771-122">Request headers</span></span>

| <span data-ttu-id="38771-123">名称</span><span class="sxs-lookup"><span data-stu-id="38771-123">Name</span></span>           | <span data-ttu-id="38771-124">说明</span><span class="sxs-lookup"><span data-stu-id="38771-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="38771-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="38771-125">Authorization</span></span>  | <span data-ttu-id="38771-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38771-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38771-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="38771-128">Request body</span></span>

<span data-ttu-id="38771-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38771-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38771-130">响应</span><span class="sxs-lookup"><span data-stu-id="38771-130">Response</span></span>

<span data-ttu-id="38771-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="38771-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38771-132">示例</span><span class="sxs-lookup"><span data-stu-id="38771-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="38771-133">请求</span><span class="sxs-lookup"><span data-stu-id="38771-133">Request</span></span>

<span data-ttu-id="38771-134">下面的示例演示了检索已授予给定资源服务主体的应用程序角色分配的请求。</span><span class="sxs-lookup"><span data-stu-id="38771-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo
```

### <a name="response"></a><span data-ttu-id="38771-135">响应</span><span class="sxs-lookup"><span data-stu-id="38771-135">Response</span></span>

<span data-ttu-id="38771-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="38771-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="38771-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="38771-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
