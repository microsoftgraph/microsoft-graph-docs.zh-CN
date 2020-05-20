---
title: 删除向用户授予的 appRoleAssignment
description: 删除已向用户授予的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 447d635a6822fb62d9be128b46c357ac6efa06df
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290066"
---
# <a name="delete-an-approleassignment-granted-to-a-user"></a><span data-ttu-id="f392d-103">删除向用户授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f392d-103">Delete an appRoleAssignment granted to a user</span></span>

<span data-ttu-id="f392d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f392d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f392d-105">删除已向用户授予的[appRoleAssignment](../resources/approleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="f392d-105">Delete an [appRoleAssignment](../resources/approleassignment.md) that has been granted to a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f392d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f392d-106">Permissions</span></span>

<span data-ttu-id="f392d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f392d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f392d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f392d-109">Permission type</span></span>      | <span data-ttu-id="f392d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f392d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f392d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f392d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f392d-112">AppRoleAssignment、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="f392d-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f392d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f392d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f392d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f392d-114">Not supported.</span></span>    |
|<span data-ttu-id="f392d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f392d-115">Application</span></span> | <span data-ttu-id="f392d-116">AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f392d-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f392d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f392d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="f392d-118">作为一种最佳做法，我们建议通过 `appRoleAssignedTo` _资源_服务主体的关系（而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系）删除应用程序角色分配。</span><span class="sxs-lookup"><span data-stu-id="f392d-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f392d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f392d-119">Request headers</span></span>

| <span data-ttu-id="f392d-120">名称</span><span class="sxs-lookup"><span data-stu-id="f392d-120">Name</span></span>       | <span data-ttu-id="f392d-121">类型</span><span class="sxs-lookup"><span data-stu-id="f392d-121">Type</span></span> | <span data-ttu-id="f392d-122">说明</span><span class="sxs-lookup"><span data-stu-id="f392d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f392d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f392d-123">Authorization</span></span>  | <span data-ttu-id="f392d-124">string</span><span class="sxs-lookup"><span data-stu-id="f392d-124">string</span></span>  | <span data-ttu-id="f392d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f392d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f392d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f392d-127">Request body</span></span>

<span data-ttu-id="f392d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f392d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f392d-129">响应</span><span class="sxs-lookup"><span data-stu-id="f392d-129">Response</span></span>

<span data-ttu-id="f392d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f392d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f392d-132">示例</span><span class="sxs-lookup"><span data-stu-id="f392d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f392d-133">请求</span><span class="sxs-lookup"><span data-stu-id="f392d-133">Request</span></span>

<span data-ttu-id="f392d-134">下面的示例展示了删除应用程序角色分配的请求。</span><span class="sxs-lookup"><span data-stu-id="f392d-134">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/appRoleAssignments/{id}
```

### <a name="response"></a><span data-ttu-id="f392d-135">响应</span><span class="sxs-lookup"><span data-stu-id="f392d-135">Response</span></span>

<span data-ttu-id="f392d-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f392d-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
