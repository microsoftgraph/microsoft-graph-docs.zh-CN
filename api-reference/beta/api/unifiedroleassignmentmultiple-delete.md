---
title: 删除 unifiedRoleAssignmentMultiple
description: 删除 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 476f9a0dc37d919ea2977602298a4b438bbd1956
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334568"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="ac231-103">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="ac231-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="ac231-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac231-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac231-105">删除 RBAC 提供程序的 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac231-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="ac231-106">这适用于支持多个主体和范围的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="ac231-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="ac231-107">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="ac231-107">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="ac231-108">云电脑</span><span class="sxs-lookup"><span data-stu-id="ac231-108">cloud PC</span></span> 
- <span data-ttu-id="ac231-109">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="ac231-109">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ac231-110">权限</span><span class="sxs-lookup"><span data-stu-id="ac231-110">Permissions</span></span>

<span data-ttu-id="ac231-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="ac231-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="ac231-112">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac231-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="ac231-113">对于云电脑提供商</span><span class="sxs-lookup"><span data-stu-id="ac231-113">For Cloud PC provider</span></span>

|<span data-ttu-id="ac231-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac231-114">Permission type</span></span>      | <span data-ttu-id="ac231-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac231-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac231-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac231-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="ac231-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac231-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="ac231-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac231-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac231-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac231-119">Not supported.</span></span>    |
|<span data-ttu-id="ac231-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac231-120">Application</span></span> | <span data-ttu-id="ac231-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac231-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="ac231-122">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="ac231-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="ac231-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac231-123">Permission type</span></span>      | <span data-ttu-id="ac231-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac231-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac231-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac231-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="ac231-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac231-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="ac231-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac231-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac231-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac231-128">Not supported.</span></span>    |
|<span data-ttu-id="ac231-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac231-129">Application</span></span> | <span data-ttu-id="ac231-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac231-130">DeviceManagementRBAC.ReadWrite.All</span></span> |



## <a name="http-request"></a><span data-ttu-id="ac231-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac231-131">HTTP request</span></span>

<span data-ttu-id="ac231-132">若要删除云电脑提供商的 unifiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="ac231-132">To delete a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="ac231-133">若要删除 Intune 提供程序的 unifiedRoleAssignmentMultiple：</span><span class="sxs-lookup"><span data-stu-id="ac231-133">To delete a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ac231-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac231-134">Request headers</span></span>

| <span data-ttu-id="ac231-135">名称</span><span class="sxs-lookup"><span data-stu-id="ac231-135">Name</span></span> | <span data-ttu-id="ac231-136">说明</span><span class="sxs-lookup"><span data-stu-id="ac231-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ac231-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac231-137">Authorization</span></span> | <span data-ttu-id="ac231-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ac231-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac231-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac231-139">Request body</span></span>

<span data-ttu-id="ac231-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac231-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac231-141">响应</span><span class="sxs-lookup"><span data-stu-id="ac231-141">Response</span></span>

<span data-ttu-id="ac231-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ac231-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac231-144">示例</span><span class="sxs-lookup"><span data-stu-id="ac231-144">Example</span></span>

### <a name="example-1-delete-a-unifiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="ac231-145">示例 1：删除 Intune 提供程序中的 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="ac231-145">Example 1: Delete a unifiedRoleAssignmentMultiple in an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="ac231-146">请求</span><span class="sxs-lookup"><span data-stu-id="ac231-146">Request</span></span>

<span data-ttu-id="ac231-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac231-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ac231-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac231-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="ac231-149">C#</span><span class="sxs-lookup"><span data-stu-id="ac231-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac231-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac231-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac231-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac231-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac231-152">Java</span><span class="sxs-lookup"><span data-stu-id="ac231-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac231-153">响应</span><span class="sxs-lookup"><span data-stu-id="ac231-153">Response</span></span>

<span data-ttu-id="ac231-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac231-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-delete-a-unifiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="ac231-155">示例 2：删除云电脑提供商中的 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="ac231-155">Example 2: Delete a unifiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="ac231-156">请求</span><span class="sxs-lookup"><span data-stu-id="ac231-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ac231-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac231-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/id
```
# <a name="c"></a>[<span data-ttu-id="ac231-158">C#</span><span class="sxs-lookup"><span data-stu-id="ac231-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac231-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac231-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac231-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac231-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac231-161">Java</span><span class="sxs-lookup"><span data-stu-id="ac231-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ac231-162">响应</span><span class="sxs-lookup"><span data-stu-id="ac231-162">Response</span></span>

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


