---
title: 删除为服务主体授予的 appRoleAssignment
description: 删除为服务主体授予的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: cbb66a092a8d10aed2c063ac82b1ea19ca4dd1b1
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383439"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="9edd6-103">删除为服务主体授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9edd6-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="9edd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9edd6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9edd6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9edd6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9edd6-106">删除已授予某个资源服务主体的用户、组或客户端服务主体的[appRoleAssignment](../resources/approleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="9edd6-106">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="9edd6-107">权限</span><span class="sxs-lookup"><span data-stu-id="9edd6-107">Permissions</span></span>

<span data-ttu-id="9edd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9edd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9edd6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9edd6-110">Permission type</span></span>      | <span data-ttu-id="9edd6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9edd6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9edd6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9edd6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9edd6-113">AppRoleAssignment、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="9edd6-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9edd6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9edd6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9edd6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9edd6-115">Not supported.</span></span>    |
|<span data-ttu-id="9edd6-116">Application</span><span class="sxs-lookup"><span data-stu-id="9edd6-116">Application</span></span> | <span data-ttu-id="9edd6-117">AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9edd6-117">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9edd6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9edd6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}
```

> [!NOTE]
> <span data-ttu-id="9edd6-119">作为一种最佳做法，我们建议通过 `appRoleAssignedTo` _资源_服务主体的关系（而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系）删除应用程序角色分配。</span><span class="sxs-lookup"><span data-stu-id="9edd6-119">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9edd6-120">请求头</span><span class="sxs-lookup"><span data-stu-id="9edd6-120">Request headers</span></span>

| <span data-ttu-id="9edd6-121">名称</span><span class="sxs-lookup"><span data-stu-id="9edd6-121">Name</span></span>       | <span data-ttu-id="9edd6-122">类型</span><span class="sxs-lookup"><span data-stu-id="9edd6-122">Type</span></span> | <span data-ttu-id="9edd6-123">说明</span><span class="sxs-lookup"><span data-stu-id="9edd6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9edd6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9edd6-124">Authorization</span></span>  | <span data-ttu-id="9edd6-125">string</span><span class="sxs-lookup"><span data-stu-id="9edd6-125">string</span></span>  | <span data-ttu-id="9edd6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9edd6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9edd6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9edd6-128">Request body</span></span>

<span data-ttu-id="9edd6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9edd6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9edd6-130">响应</span><span class="sxs-lookup"><span data-stu-id="9edd6-130">Response</span></span>

<span data-ttu-id="9edd6-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9edd6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9edd6-133">示例</span><span class="sxs-lookup"><span data-stu-id="9edd6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9edd6-134">请求</span><span class="sxs-lookup"><span data-stu-id="9edd6-134">Request</span></span>

<span data-ttu-id="9edd6-135">下面的示例展示了从资源服务主体中删除应用程序角色分配的请求。</span><span class="sxs-lookup"><span data-stu-id="9edd6-135">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="9edd6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9edd6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="9edd6-137">C#</span><span class="sxs-lookup"><span data-stu-id="9edd6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9edd6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9edd6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9edd6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9edd6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9edd6-140">响应</span><span class="sxs-lookup"><span data-stu-id="9edd6-140">Response</span></span>

<span data-ttu-id="9edd6-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9edd6-141">The following is an example of the response.</span></span>

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
