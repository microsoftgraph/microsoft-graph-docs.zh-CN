---
title: 向服务主体授予 appRoleAssignment
description: 向服务主体授予应用角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 3eab61ceab9b171d1cec41f2f396ddaafe767eff
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955462"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="e5725-103">向服务主体授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e5725-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="e5725-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5725-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5725-105">向客户端服务主体分配一个应用角色。</span><span class="sxs-lookup"><span data-stu-id="e5725-105">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="e5725-106">分配给服务主体的应用角色也被称为[应用程序权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。</span><span class="sxs-lookup"><span data-stu-id="e5725-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="e5725-107">应用程序权限可以通过应用角色分配直接授予，或通过[协议体验](/azure/active-directory/develop/application-consent-experience)授予。</span><span class="sxs-lookup"><span data-stu-id="e5725-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="e5725-108">若要向客户端服务主体授予应用角色分配，需使用三个标识符：</span><span class="sxs-lookup"><span data-stu-id="e5725-108">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="e5725-109">`principalId`： 或要向其分配应用角色的客户端服务主体的 `id`。</span><span class="sxs-lookup"><span data-stu-id="e5725-109">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="e5725-110">`resourceId`：已定义应用角色（应用程序权限）的资源 `servicePrincipal` (API) 的 `id`。</span><span class="sxs-lookup"><span data-stu-id="e5725-110">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="e5725-111">`appRoleId`：要分配给客户端服务主体的 `appRole`（在资源服务主体上定义）的 `id`。</span><span class="sxs-lookup"><span data-stu-id="e5725-111">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5725-112">权限</span><span class="sxs-lookup"><span data-stu-id="e5725-112">Permissions</span></span>

<span data-ttu-id="e5725-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5725-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5725-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5725-115">Permission type</span></span>      | <span data-ttu-id="e5725-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5725-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5725-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5725-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e5725-118">AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5725-118">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5725-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5725-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5725-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5725-120">Not supported.</span></span>    |
|<span data-ttu-id="e5725-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5725-121">Application</span></span> | <span data-ttu-id="e5725-122">AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5725-122">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5725-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5725-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="e5725-124">最佳做法是，建议通过 [`appRoleAssignedTo`_资源_ 服务主体](serviceprincipal-post-approleassignedto.md)的关系（而不是通过分配的用户、组或服务主体的`appRoleAssignments`关系）创建应用角色分配。</span><span class="sxs-lookup"><span data-stu-id="e5725-124">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5725-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5725-125">Request headers</span></span>

| <span data-ttu-id="e5725-126">名称</span><span class="sxs-lookup"><span data-stu-id="e5725-126">Name</span></span>       | <span data-ttu-id="e5725-127">说明</span><span class="sxs-lookup"><span data-stu-id="e5725-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e5725-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5725-128">Authorization</span></span> | <span data-ttu-id="e5725-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5725-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5725-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="e5725-131">Content-type</span></span> | <span data-ttu-id="e5725-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5725-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5725-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5725-134">Request body</span></span>

<span data-ttu-id="e5725-135">在请求正文中，提供 [appRoleAssignment](../resources/approleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5725-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e5725-136">响应</span><span class="sxs-lookup"><span data-stu-id="e5725-136">Response</span></span>

<span data-ttu-id="e5725-137">如果成功，此运营商将在响应正文中返回 `201 Created` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5725-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5725-138">示例</span><span class="sxs-lookup"><span data-stu-id="e5725-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5725-139">请求</span><span class="sxs-lookup"><span data-stu-id="e5725-139">Request</span></span>

<span data-ttu-id="e5725-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5725-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5725-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5725-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment_2"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignments
Content-Type: application/json

{
  "principalId": "8fce32da-1246-437b-99cd-76d1d4677bd5",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
}
```
# <a name="c"></a>[<span data-ttu-id="e5725-142">C#</span><span class="sxs-lookup"><span data-stu-id="e5725-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5725-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5725-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5725-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5725-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5725-145">Java</span><span class="sxs-lookup"><span data-stu-id="e5725-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e5725-146">在此示例中，`{id}` 和 `{principalId-value}` 都将成为已分配的客户端服务主体的 `id`，`{resourceId}` 将成为资源服务主体 (API) 的 `id`。</span><span class="sxs-lookup"><span data-stu-id="e5725-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned client service principal, and `{resourceId}` would be the `id` of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="e5725-147">响应</span><span class="sxs-lookup"><span data-stu-id="e5725-147">Response</span></span>

<span data-ttu-id="e5725-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5725-148">Here is an example of the response.</span></span> 

> <span data-ttu-id="e5725-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5725-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
  "id": "2jLOj0YSe0OZzXbR1Gd71fDqFUrPM1xIgUfvWBHJ9n0",
  "creationTimestamp": "2021-02-15T16:39:38.2975029Z",
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7",
  "principalDisplayName": "Remote living",
  "principalId": "8fce32da-1246-437b-99cd-76d1d4677bd5",
  "principalType": "Group",
  "resourceDisplayName": "Yammer",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
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

