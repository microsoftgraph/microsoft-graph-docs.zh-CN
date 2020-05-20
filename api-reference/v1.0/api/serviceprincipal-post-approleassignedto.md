---
title: 向服务主体授予 appRoleAssignment
description: 向服务主体授予应用程序角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: da758c233854d3569e9ac4b9db8c88c74f77f92e
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289493"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a><span data-ttu-id="d7157-103">为服务主体授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d7157-103">Grant an appRoleAssignment for a service principal</span></span>

<span data-ttu-id="d7157-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7157-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d7157-105">将资源服务主体的应用程序角色分配给用户、组或客户端服务主体。</span><span class="sxs-lookup"><span data-stu-id="d7157-105">Assign an app role for a resource service principal, to a user, group, or client service principal.</span></span>

<span data-ttu-id="d7157-106">分配给服务主体的应用程序角色也称为 "[应用程序权限](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types)"。</span><span class="sxs-lookup"><span data-stu-id="d7157-106">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="d7157-107">可以通过应用角色分配或通过[许可体验](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience)直接授予应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="d7157-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="d7157-108">若要授予应用程序角色分配，需要三个标识符：</span><span class="sxs-lookup"><span data-stu-id="d7157-108">To grant an app role assignment, you need three identifiers:</span></span>

- <span data-ttu-id="d7157-109">`principalId`：要 `id` 向其分配应用程序角色的**用户**、**组**或客户端**servicePrincipal**的。</span><span class="sxs-lookup"><span data-stu-id="d7157-109">`principalId`: The `id` of the **user**, **group** or client **servicePrincipal** to which you are assigning the app role.</span></span>
- <span data-ttu-id="d7157-110">`resourceId`： `id` 定义了应用程序角色的资源**servicePrincipal**的。</span><span class="sxs-lookup"><span data-stu-id="d7157-110">`resourceId`: The `id` of the resource **servicePrincipal** which has defined the app role.</span></span>
- <span data-ttu-id="d7157-111">`appRoleId`： `id` 要分配给用户、组或服务主体的**appRole** （在资源服务主体上定义）的。</span><span class="sxs-lookup"><span data-stu-id="d7157-111">`appRoleId`: The `id` of the **appRole** (defined on the resource service principal) to assign to a user, group, or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7157-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="d7157-112">Permissions</span></span>

<span data-ttu-id="d7157-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7157-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7157-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7157-115">Permission type</span></span>      | <span data-ttu-id="d7157-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7157-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7157-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7157-117">Delegated (work or school account)</span></span> | <span data-ttu-id="d7157-118">AppRoleAssignment、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="d7157-118">AppRoleAssignment.ReadWrite.All,Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7157-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7157-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7157-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7157-120">Not supported.</span></span>    |
|<span data-ttu-id="d7157-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7157-121">Application</span></span> | <span data-ttu-id="d7157-122">AppRoleAssignment，</span><span class="sxs-lookup"><span data-stu-id="d7157-122">AppRoleAssignment.ReadWrite.All,</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7157-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7157-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a><span data-ttu-id="d7157-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7157-124">Request headers</span></span>

| <span data-ttu-id="d7157-125">名称</span><span class="sxs-lookup"><span data-stu-id="d7157-125">Name</span></span>       | <span data-ttu-id="d7157-126">说明</span><span class="sxs-lookup"><span data-stu-id="d7157-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="d7157-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7157-127">Authorization</span></span> | <span data-ttu-id="d7157-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7157-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7157-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="d7157-130">Content-type</span></span> | <span data-ttu-id="d7157-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d7157-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7157-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7157-133">Request body</span></span>

<span data-ttu-id="d7157-134">在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7157-134">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d7157-135">响应</span><span class="sxs-lookup"><span data-stu-id="d7157-135">Response</span></span>

<span data-ttu-id="d7157-136">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7157-136">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7157-137">示例</span><span class="sxs-lookup"><span data-stu-id="d7157-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7157-138">请求</span><span class="sxs-lookup"><span data-stu-id="d7157-138">Request</span></span>

<span data-ttu-id="d7157-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7157-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignedTo
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```

<span data-ttu-id="d7157-140">在此示例中， `{id}` 和 `{resourceId-value}` 都是 `id` 资源服务主体的，并且 `{principalId}` 是分配的 `id` 用户、组或客户端服务主体的。</span><span class="sxs-lookup"><span data-stu-id="d7157-140">In this example, `{id}` and `{resourceId-value}` would both be the `id` of the resource service principal, and `{principalId}` would be the `id` of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="d7157-141">响应</span><span class="sxs-lookup"><span data-stu-id="d7157-141">Response</span></span>

<span data-ttu-id="d7157-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d7157-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="d7157-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d7157-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
