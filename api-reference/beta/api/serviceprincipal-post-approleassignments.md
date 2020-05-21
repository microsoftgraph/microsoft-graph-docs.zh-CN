---
title: 向服务主体授予 appRoleAssignment
description: 向服务主体授予应用程序角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: f28dff8e697cba37897f0f4124c3f40e9fab5593
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336032"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="c7162-103">向服务主体授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c7162-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="c7162-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7162-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7162-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7162-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7162-106">将应用程序角色分配给客户端服务主体。</span><span class="sxs-lookup"><span data-stu-id="c7162-106">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="c7162-107">分配给服务主体的应用程序角色也称为 "[应用程序权限](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types)"。</span><span class="sxs-lookup"><span data-stu-id="c7162-107">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="c7162-108">可以通过应用角色分配或通过[许可体验](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience)直接授予应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="c7162-108">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="c7162-109">若要向客户端服务主体授予应用程序角色分配，您需要三个标识符：</span><span class="sxs-lookup"><span data-stu-id="c7162-109">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="c7162-110">`principalId`：要 `id` 向其分配应用角色的客户端服务主体的。</span><span class="sxs-lookup"><span data-stu-id="c7162-110">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="c7162-111">`resourceId`： `id` `servicePrincipal` 定义了应用程序角色（应用程序权限）的资源（API）。</span><span class="sxs-lookup"><span data-stu-id="c7162-111">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="c7162-112">`appRoleId`： `id` `appRole` 要分配给客户端服务主体的（在资源服务主体上定义）的。</span><span class="sxs-lookup"><span data-stu-id="c7162-112">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7162-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7162-113">Permissions</span></span>

<span data-ttu-id="c7162-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7162-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7162-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7162-116">Permission type</span></span>      | <span data-ttu-id="c7162-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7162-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7162-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7162-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c7162-119">AppRoleAssignment、Directory.accessasuser.all、all 和的所有子目录</span><span class="sxs-lookup"><span data-stu-id="c7162-119">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c7162-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7162-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7162-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7162-121">Not supported.</span></span>    |
|<span data-ttu-id="c7162-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7162-122">Application</span></span> | <span data-ttu-id="c7162-123">AppRoleAssignment、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="c7162-123">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7162-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7162-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="c7162-125">作为一种最佳做法，我们建议通过[ `appRoleAssignedTo` _资源_服务主体的关系](serviceprincipal-post-approleassignedto.md)创建应用程序角色分配，而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系。</span><span class="sxs-lookup"><span data-stu-id="c7162-125">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7162-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7162-126">Request headers</span></span>

| <span data-ttu-id="c7162-127">名称</span><span class="sxs-lookup"><span data-stu-id="c7162-127">Name</span></span>       | <span data-ttu-id="c7162-128">说明</span><span class="sxs-lookup"><span data-stu-id="c7162-128">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c7162-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7162-129">Authorization</span></span> | <span data-ttu-id="c7162-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7162-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c7162-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="c7162-132">Content-type</span></span> | <span data-ttu-id="c7162-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c7162-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7162-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7162-135">Request body</span></span>

<span data-ttu-id="c7162-136">在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7162-136">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c7162-137">响应</span><span class="sxs-lookup"><span data-stu-id="c7162-137">Response</span></span>

<span data-ttu-id="c7162-138">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7162-138">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7162-139">示例</span><span class="sxs-lookup"><span data-stu-id="c7162-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7162-140">请求</span><span class="sxs-lookup"><span data-stu-id="c7162-140">Request</span></span>

<span data-ttu-id="c7162-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7162-141">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7162-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7162-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c7162-143">C#</span><span class="sxs-lookup"><span data-stu-id="c7162-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7162-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7162-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7162-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7162-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c7162-146">在此示例中， `{id}` 和 `{principalId-value}` 都是 `id` 分配的客户端服务主体，也是 `{resoruceId}` `id` 资源服务主体（API）的。</span><span class="sxs-lookup"><span data-stu-id="c7162-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned client service principal, and `{resoruceId}` would be the `id` of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="c7162-147">响应</span><span class="sxs-lookup"><span data-stu-id="c7162-147">Response</span></span>

<span data-ttu-id="c7162-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c7162-148">Here is an example of the response.</span></span> 

> <span data-ttu-id="c7162-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7162-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
