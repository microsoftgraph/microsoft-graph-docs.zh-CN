---
title: 删除为服务主体授予的 appRoleAssignment
description: 删除为服务主体授予的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f1d874ee77733d81da3a94f448f57675c15062bc
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317040"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="7c440-103">删除为服务主体授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7c440-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="7c440-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c440-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c440-105">删除已授予资源服务主体的用户、组或客户端服务主体的[appRoleAssignment。](../resources/approleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c440-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c440-106">权限</span><span class="sxs-lookup"><span data-stu-id="7c440-106">Permissions</span></span>

<span data-ttu-id="7c440-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c440-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c440-109">Permission type</span></span>      | <span data-ttu-id="7c440-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c440-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c440-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c440-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7c440-112">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7c440-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7c440-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c440-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c440-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c440-114">Not supported.</span></span>    |
|<span data-ttu-id="7c440-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c440-115">Application</span></span> | <span data-ttu-id="7c440-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c440-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c440-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c440-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="7c440-118">作为最佳实践，我们建议通过资源服务主体的关系（而不是分配的用户、组或服务主体的关系）删除应用程序 `appRoleAssignedTo`  `appRoleAssignments` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="7c440-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c440-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c440-119">Request headers</span></span>

| <span data-ttu-id="7c440-120">名称</span><span class="sxs-lookup"><span data-stu-id="7c440-120">Name</span></span>       | <span data-ttu-id="7c440-121">类型</span><span class="sxs-lookup"><span data-stu-id="7c440-121">Type</span></span> | <span data-ttu-id="7c440-122">说明</span><span class="sxs-lookup"><span data-stu-id="7c440-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c440-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c440-123">Authorization</span></span>  | <span data-ttu-id="7c440-124">string</span><span class="sxs-lookup"><span data-stu-id="7c440-124">string</span></span>  | <span data-ttu-id="7c440-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c440-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c440-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c440-127">Request body</span></span>

<span data-ttu-id="7c440-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c440-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c440-129">响应</span><span class="sxs-lookup"><span data-stu-id="7c440-129">Response</span></span>

<span data-ttu-id="7c440-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c440-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c440-132">示例</span><span class="sxs-lookup"><span data-stu-id="7c440-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c440-133">请求</span><span class="sxs-lookup"><span data-stu-id="7c440-133">Request</span></span>

<span data-ttu-id="7c440-134">下面是从资源服务主体角色分配应用程序请求的示例。</span><span class="sxs-lookup"><span data-stu-id="7c440-134">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```


<span data-ttu-id="7c440-135">此示例中 为资源服务主体的 `{resource-SP-id}` ID，是 appRoleAssignment 对象的 ID，该对象表示用户、组或客户端服务主体的 `{appRoleAssignment-id}` 分配。</span><span class="sxs-lookup"><span data-stu-id="7c440-135">In this example, `{resource-SP-id}` is the id of the resource service principal, and `{appRoleAssignment-id}` is the id of the appRoleAssignment object that represents an assignment to the user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="7c440-136">响应</span><span class="sxs-lookup"><span data-stu-id="7c440-136">Response</span></span>

<span data-ttu-id="7c440-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c440-137">The following is an example of the response.</span></span>

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

