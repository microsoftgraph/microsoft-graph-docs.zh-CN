---
title: 从服务主体中删除 appRoleAssignment
description: 从服务主体中删除 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 8e4f2c986723c8dab08eab88b6b80f5f72d6f76c
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703578"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="beaf9-103">删除授予服务主体的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="beaf9-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="beaf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beaf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beaf9-105">删除已授予服务主体的[appRoleAssignment。](../resources/approleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="beaf9-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="beaf9-106">分配给服务主体的应用程序角色也称为应用程序 [权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。</span><span class="sxs-lookup"><span data-stu-id="beaf9-106">App roles which are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="beaf9-107">删除服务角色分配应用程序权限等效于撤销仅应用程序权限授予。</span><span class="sxs-lookup"><span data-stu-id="beaf9-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="beaf9-108">权限</span><span class="sxs-lookup"><span data-stu-id="beaf9-108">Permissions</span></span>

<span data-ttu-id="beaf9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="beaf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beaf9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="beaf9-111">Permission type</span></span>      | <span data-ttu-id="beaf9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="beaf9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beaf9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="beaf9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="beaf9-114">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="beaf9-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="beaf9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="beaf9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beaf9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="beaf9-116">Not supported.</span></span>    |
|<span data-ttu-id="beaf9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="beaf9-117">Application</span></span> | <span data-ttu-id="beaf9-118">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beaf9-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="beaf9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="beaf9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="beaf9-120">作为最佳实践，我们建议通过资源服务主体的关系（而不是分配的用户、组或服务主体的关系）删除应用程序 `appRoleAssignedTo`  `appRoleAssignments` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="beaf9-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="beaf9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="beaf9-121">Request headers</span></span>

| <span data-ttu-id="beaf9-122">名称</span><span class="sxs-lookup"><span data-stu-id="beaf9-122">Name</span></span>       | <span data-ttu-id="beaf9-123">类型</span><span class="sxs-lookup"><span data-stu-id="beaf9-123">Type</span></span> | <span data-ttu-id="beaf9-124">说明</span><span class="sxs-lookup"><span data-stu-id="beaf9-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="beaf9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="beaf9-125">Authorization</span></span>  | <span data-ttu-id="beaf9-126">string</span><span class="sxs-lookup"><span data-stu-id="beaf9-126">string</span></span>  | <span data-ttu-id="beaf9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="beaf9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beaf9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="beaf9-129">Request body</span></span>

<span data-ttu-id="beaf9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="beaf9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beaf9-131">响应</span><span class="sxs-lookup"><span data-stu-id="beaf9-131">Response</span></span>

<span data-ttu-id="beaf9-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="beaf9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="beaf9-134">示例</span><span class="sxs-lookup"><span data-stu-id="beaf9-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="beaf9-135">请求</span><span class="sxs-lookup"><span data-stu-id="beaf9-135">Request</span></span>

<span data-ttu-id="beaf9-136">下面是一个请求删除应用示例角色分配。</span><span class="sxs-lookup"><span data-stu-id="beaf9-136">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```

### <a name="response"></a><span data-ttu-id="beaf9-137">响应</span><span class="sxs-lookup"><span data-stu-id="beaf9-137">Response</span></span>

<span data-ttu-id="beaf9-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="beaf9-138">The following is an example of the response.</span></span>

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
