---
title: 删除为服务主体授予的 appRoleAssignment
description: 删除为服务主体授予的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 8983149857caaf80602da99b835d4a63a36e25ae
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317082"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="2b28f-103">删除为服务主体授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b28f-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="2b28f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b28f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b28f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b28f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b28f-106">删除已授予资源服务主体的用户、组或客户端服务主体的[appRoleAssignment。](../resources/approleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2b28f-106">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b28f-107">权限</span><span class="sxs-lookup"><span data-stu-id="2b28f-107">Permissions</span></span>

<span data-ttu-id="2b28f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b28f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b28f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b28f-110">Permission type</span></span>      | <span data-ttu-id="2b28f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b28f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b28f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b28f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b28f-113">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b28f-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b28f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b28f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b28f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b28f-115">Not supported.</span></span>    |
|<span data-ttu-id="2b28f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b28f-116">Application</span></span> | <span data-ttu-id="2b28f-117">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b28f-117">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b28f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b28f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="2b28f-119">作为最佳实践，我们建议通过资源服务主体的关系（而不是分配的用户、组或服务主体的关系）删除应用程序 `appRoleAssignedTo`  `appRoleAssignments` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="2b28f-119">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b28f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b28f-120">Request headers</span></span>

| <span data-ttu-id="2b28f-121">名称</span><span class="sxs-lookup"><span data-stu-id="2b28f-121">Name</span></span>       | <span data-ttu-id="2b28f-122">类型</span><span class="sxs-lookup"><span data-stu-id="2b28f-122">Type</span></span> | <span data-ttu-id="2b28f-123">说明</span><span class="sxs-lookup"><span data-stu-id="2b28f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2b28f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b28f-124">Authorization</span></span>  | <span data-ttu-id="2b28f-125">string</span><span class="sxs-lookup"><span data-stu-id="2b28f-125">string</span></span>  | <span data-ttu-id="2b28f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b28f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b28f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b28f-128">Request body</span></span>

<span data-ttu-id="2b28f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b28f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b28f-130">响应</span><span class="sxs-lookup"><span data-stu-id="2b28f-130">Response</span></span>

<span data-ttu-id="2b28f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2b28f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b28f-133">示例</span><span class="sxs-lookup"><span data-stu-id="2b28f-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b28f-134">请求</span><span class="sxs-lookup"><span data-stu-id="2b28f-134">Request</span></span>

<span data-ttu-id="2b28f-135">下面是从资源服务主体角色分配应用程序请求的示例。</span><span class="sxs-lookup"><span data-stu-id="2b28f-135">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```

<span data-ttu-id="2b28f-136">此示例中 为资源服务主体的 `{resource-SP-id}` ID，是 appRoleAssignment 对象的 ID，该对象表示用户、组或客户端服务主体的 `{appRoleAssignment-id}` 分配。</span><span class="sxs-lookup"><span data-stu-id="2b28f-136">In this example, `{resource-SP-id}` is the id of the resource service principal, and `{appRoleAssignment-id}` is the id of the appRoleAssignment object that represents an assignment to the user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="2b28f-137">响应</span><span class="sxs-lookup"><span data-stu-id="2b28f-137">Response</span></span>

<span data-ttu-id="2b28f-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2b28f-138">The following is an example of the response.</span></span>

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



