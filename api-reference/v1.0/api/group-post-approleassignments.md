---
title: 向组授予 appRoleAssignment
description: 向组授予应用角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: e17f94e0b1d62015bfbff8d849c4d205a48cba2a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949922"
---
# <a name="grant-an-approleassignment-to-a-group"></a><span data-ttu-id="3564c-103">向组授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3564c-103">Grant an appRoleAssignment to a group</span></span>

<span data-ttu-id="3564c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3564c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3564c-105">使用此 API 将应用角色分配给组。</span><span class="sxs-lookup"><span data-stu-id="3564c-105">Use this API to assign an app role to a group.</span></span> <span data-ttu-id="3564c-106">该组的所有直接成员都将被视为已分配。</span><span class="sxs-lookup"><span data-stu-id="3564c-106">All direct members of the group will be considered assigned.</span></span> <span data-ttu-id="3564c-107">若要向组授予应用角色分配，需使用三个标识符：</span><span class="sxs-lookup"><span data-stu-id="3564c-107">To grant an app role assignment to a group, you need three identifiers:</span></span>

- <span data-ttu-id="3564c-108">`principalId`：要向其分配应用角色的组的 `id`。</span><span class="sxs-lookup"><span data-stu-id="3564c-108">`principalId`: The `id` of the group to which you are assigning the app role.</span></span>
- <span data-ttu-id="3564c-109">`resourceId`：已定义应用角色的资源 `servicePrincipal` 的 `id`。</span><span class="sxs-lookup"><span data-stu-id="3564c-109">`resourceId`: The `id` of the resource `servicePrincipal` which has defined the app role.</span></span>
- <span data-ttu-id="3564c-110">`appRoleId`：要分配给组的 `appRole`（在资源服务主体上定义）的 `id`。</span><span class="sxs-lookup"><span data-stu-id="3564c-110">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the group.</span></span>

<span data-ttu-id="3564c-111">要[使用组来管理对应用程序的访问](/azure/active-directory/users-groups-roles/groups-saasapps)，可能还需要其他许可证。</span><span class="sxs-lookup"><span data-stu-id="3564c-111">Additional licenses might be required to [use a group to manage access to applications](/azure/active-directory/users-groups-roles/groups-saasapps).</span></span>

## <a name="permissions"></a><span data-ttu-id="3564c-112">权限</span><span class="sxs-lookup"><span data-stu-id="3564c-112">Permissions</span></span>

<span data-ttu-id="3564c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3564c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3564c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="3564c-115">Permission type</span></span>      | <span data-ttu-id="3564c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3564c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3564c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3564c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="3564c-118">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3564c-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3564c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3564c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3564c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="3564c-120">Not supported.</span></span>    |
|<span data-ttu-id="3564c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="3564c-121">Application</span></span> | <span data-ttu-id="3564c-122">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3564c-122">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3564c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3564c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="3564c-124">最佳做法是，建议通过 _资源_ 服务主体的 `appRoleAssignedTo` 关系（而不是通过分配的用户、组或服务主体的 `appRoleAssignments` 关系）创建应用角色分配。</span><span class="sxs-lookup"><span data-stu-id="3564c-124">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3564c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="3564c-125">Request headers</span></span>

| <span data-ttu-id="3564c-126">名称</span><span class="sxs-lookup"><span data-stu-id="3564c-126">Name</span></span>       | <span data-ttu-id="3564c-127">说明</span><span class="sxs-lookup"><span data-stu-id="3564c-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="3564c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="3564c-128">Authorization</span></span> | <span data-ttu-id="3564c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3564c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3564c-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="3564c-131">Content-type</span></span> | <span data-ttu-id="3564c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3564c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3564c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="3564c-134">Request body</span></span>

<span data-ttu-id="3564c-135">在请求正文中，提供 [appRoleAssignment](../resources/approleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3564c-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3564c-136">响应</span><span class="sxs-lookup"><span data-stu-id="3564c-136">Response</span></span>

<span data-ttu-id="3564c-137">如果成功，此运营商将在响应正文中返回 `201 Created` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3564c-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3564c-138">示例</span><span class="sxs-lookup"><span data-stu-id="3564c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3564c-139">请求</span><span class="sxs-lookup"><span data-stu-id="3564c-139">Request</span></span>

<span data-ttu-id="3564c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3564c-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3564c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="3564c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
Content-Type: application/json

{
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="3564c-142">C#</span><span class="sxs-lookup"><span data-stu-id="3564c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3564c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3564c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3564c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3564c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3564c-145">Java</span><span class="sxs-lookup"><span data-stu-id="3564c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3564c-146">在此示例中，`{id}` 和 `{principalId-value}` 均为已分配组的 `id`。</span><span class="sxs-lookup"><span data-stu-id="3564c-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned group.</span></span>

### <a name="response"></a><span data-ttu-id="3564c-147">响应</span><span class="sxs-lookup"><span data-stu-id="3564c-147">Response</span></span>

<span data-ttu-id="3564c-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3564c-148">Here is an example of the response.</span></span> 

><span data-ttu-id="3564c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3564c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments/$entity",
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
