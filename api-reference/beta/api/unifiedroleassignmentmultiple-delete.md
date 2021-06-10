---
title: 删除 unifiedRoleAssignmentMultiple
description: 删除 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 14ae5e8c899378e76fb201856bea2929a0ba3168
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870057"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="92656-103">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="92656-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="92656-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92656-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92656-105">删除 RBAC 提供程序的 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92656-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="92656-106">这适用于支持多个主体和范围的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="92656-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="92656-107">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="92656-107">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="92656-108">云电脑</span><span class="sxs-lookup"><span data-stu-id="92656-108">cloud PC</span></span> 
- <span data-ttu-id="92656-109">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="92656-109">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="92656-110">权限</span><span class="sxs-lookup"><span data-stu-id="92656-110">Permissions</span></span>

<span data-ttu-id="92656-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="92656-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="92656-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="92656-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="92656-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="92656-113">Supported provider</span></span>      | <span data-ttu-id="92656-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92656-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="92656-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92656-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92656-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="92656-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="92656-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="92656-117">Cloud PC</span></span> | <span data-ttu-id="92656-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92656-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="92656-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="92656-119">Not supported.</span></span> | <span data-ttu-id="92656-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92656-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="92656-121">Intune</span><span class="sxs-lookup"><span data-stu-id="92656-121">Intune</span></span> | <span data-ttu-id="92656-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92656-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="92656-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="92656-123">Not supported.</span></span>| <span data-ttu-id="92656-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92656-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92656-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92656-125">HTTP request</span></span>

<span data-ttu-id="92656-126">若要删除云电脑提供商的 unifiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="92656-126">To delete a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="92656-127">若要删除 Intune 提供程序的 unifiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="92656-127">To delete a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92656-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="92656-128">Request headers</span></span>

| <span data-ttu-id="92656-129">名称</span><span class="sxs-lookup"><span data-stu-id="92656-129">Name</span></span> | <span data-ttu-id="92656-130">说明</span><span class="sxs-lookup"><span data-stu-id="92656-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="92656-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="92656-131">Authorization</span></span> | <span data-ttu-id="92656-132">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="92656-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="92656-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="92656-133">Request body</span></span>

<span data-ttu-id="92656-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92656-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92656-135">响应</span><span class="sxs-lookup"><span data-stu-id="92656-135">Response</span></span>

<span data-ttu-id="92656-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="92656-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92656-138">示例</span><span class="sxs-lookup"><span data-stu-id="92656-138">Example</span></span>

### <a name="example-1-delete-a-unifiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="92656-139">示例 1：删除 Intune 提供程序中的 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="92656-139">Example 1: Delete a unifiedRoleAssignmentMultiple in an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="92656-140">请求</span><span class="sxs-lookup"><span data-stu-id="92656-140">Request</span></span>

<span data-ttu-id="92656-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92656-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="92656-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="92656-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="92656-143">C#</span><span class="sxs-lookup"><span data-stu-id="92656-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92656-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92656-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92656-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92656-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92656-146">Java</span><span class="sxs-lookup"><span data-stu-id="92656-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92656-147">响应</span><span class="sxs-lookup"><span data-stu-id="92656-147">Response</span></span>

<span data-ttu-id="92656-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92656-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-delete-a-unifiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="92656-149">示例 2：删除云电脑提供商中的 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="92656-149">Example 2: Delete a unifiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="92656-150">请求</span><span class="sxs-lookup"><span data-stu-id="92656-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="92656-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="92656-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/id
```
# <a name="c"></a>[<span data-ttu-id="92656-152">C#</span><span class="sxs-lookup"><span data-stu-id="92656-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92656-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92656-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92656-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92656-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92656-155">Java</span><span class="sxs-lookup"><span data-stu-id="92656-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="92656-156">响应</span><span class="sxs-lookup"><span data-stu-id="92656-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


