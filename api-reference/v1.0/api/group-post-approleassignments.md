---
title: 向组授予 appRoleAssignment
description: 向组授予应用程序角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a0c61959d8d0c47eaeda08063cc9717a26126da0
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289416"
---
# <a name="grant-an-approleassignment-to-a-group"></a><span data-ttu-id="df276-103">向组授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="df276-103">Grant an appRoleAssignment to a group</span></span>

<span data-ttu-id="df276-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df276-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df276-105">使用此 API 将应用程序角色分配给组。</span><span class="sxs-lookup"><span data-stu-id="df276-105">Use this API to assign an app role to a group.</span></span> <span data-ttu-id="df276-106">该组的所有直接成员都将被视为已分配。</span><span class="sxs-lookup"><span data-stu-id="df276-106">All direct members of the group will be considered assigned.</span></span> <span data-ttu-id="df276-107">若要向组授予应用程序角色分配，需要三个标识符：</span><span class="sxs-lookup"><span data-stu-id="df276-107">To grant an app role assignment to a group, you need three identifiers:</span></span>

- <span data-ttu-id="df276-108">`principalId`：要 `id` 向其分配应用程序角色的组的。</span><span class="sxs-lookup"><span data-stu-id="df276-108">`principalId`: The `id` of the group to which you are assigning the app role.</span></span>
- <span data-ttu-id="df276-109">`resourceId`： `id` `servicePrincipal` 定义了应用程序角色的资源的。</span><span class="sxs-lookup"><span data-stu-id="df276-109">`resourceId`: The `id` of the resource `servicePrincipal` which has defined the app role.</span></span>
- <span data-ttu-id="df276-110">`appRoleId`： `id` `appRole` 要分配给组的（在资源服务主体上定义）的。</span><span class="sxs-lookup"><span data-stu-id="df276-110">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the group.</span></span>

<span data-ttu-id="df276-111">若要[使用组来管理对应用程序的访问](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-saasapps)，可能需要其他许可证。</span><span class="sxs-lookup"><span data-stu-id="df276-111">Additional licenses might be required to [use a group to manage access to applications](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-saasapps).</span></span>

## <a name="permissions"></a><span data-ttu-id="df276-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="df276-112">Permissions</span></span>

<span data-ttu-id="df276-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df276-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df276-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="df276-115">Permission type</span></span>      | <span data-ttu-id="df276-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df276-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df276-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df276-117">Delegated (work or school account)</span></span> | <span data-ttu-id="df276-118">AppRoleAssignment、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="df276-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df276-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df276-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df276-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="df276-120">Not supported.</span></span>    |
|<span data-ttu-id="df276-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="df276-121">Application</span></span> | <span data-ttu-id="df276-122">AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="df276-122">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df276-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df276-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="df276-124">作为一种最佳做法，我们建议通过 `appRoleAssignedTo` _资源_服务主体的关系创建应用程序角色分配，而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系。</span><span class="sxs-lookup"><span data-stu-id="df276-124">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df276-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="df276-125">Request headers</span></span>

| <span data-ttu-id="df276-126">名称</span><span class="sxs-lookup"><span data-stu-id="df276-126">Name</span></span>       | <span data-ttu-id="df276-127">说明</span><span class="sxs-lookup"><span data-stu-id="df276-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="df276-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="df276-128">Authorization</span></span> | <span data-ttu-id="df276-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df276-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df276-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="df276-131">Content-type</span></span> | <span data-ttu-id="df276-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="df276-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df276-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="df276-134">Request body</span></span>

<span data-ttu-id="df276-135">在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df276-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df276-136">响应</span><span class="sxs-lookup"><span data-stu-id="df276-136">Response</span></span>

<span data-ttu-id="df276-137">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="df276-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df276-138">示例</span><span class="sxs-lookup"><span data-stu-id="df276-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df276-139">请求</span><span class="sxs-lookup"><span data-stu-id="df276-139">Request</span></span>

<span data-ttu-id="df276-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df276-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```

<span data-ttu-id="df276-141">在此示例中， `{id}` 和 `{principalId-value}` 都是 `id` 分配的组的。</span><span class="sxs-lookup"><span data-stu-id="df276-141">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned group.</span></span>

### <a name="response"></a><span data-ttu-id="df276-142">响应</span><span class="sxs-lookup"><span data-stu-id="df276-142">Response</span></span>

<span data-ttu-id="df276-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="df276-143">Here is an example of the response.</span></span> 

><span data-ttu-id="df276-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="df276-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
