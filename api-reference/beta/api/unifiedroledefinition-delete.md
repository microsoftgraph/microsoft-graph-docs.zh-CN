---
title: 删除 unifiedRoleDefinition
description: 删除 unifiedRoleDefinition 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7de16492df085b48d2fe580ff54d3cacf9dc0d22
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334365"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="9314e-103">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9314e-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="9314e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9314e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9314e-105">删除 RBAC 提供程序的 [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9314e-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="9314e-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="9314e-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="9314e-107">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="9314e-107">device management (Intune)</span></span>
- <span data-ttu-id="9314e-108">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="9314e-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="9314e-109">云电脑 RBAC 提供商当前仅支持[列表和](rbacapplication-list-roledefinitions.md)[获取](unifiedroledefinition-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="9314e-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="9314e-110">权限</span><span class="sxs-lookup"><span data-stu-id="9314e-110">Permissions</span></span>

<span data-ttu-id="9314e-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="9314e-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="9314e-112">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9314e-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="9314e-113">对于 Intune (提供程序的设备) 管理</span><span class="sxs-lookup"><span data-stu-id="9314e-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="9314e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="9314e-114">Permission type</span></span>      | <span data-ttu-id="9314e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9314e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9314e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9314e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="9314e-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9314e-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="9314e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9314e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9314e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9314e-119">Not supported.</span></span>    |
|<span data-ttu-id="9314e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="9314e-120">Application</span></span> | <span data-ttu-id="9314e-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9314e-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="9314e-122">对于 Azure AD (提供程序) 目录</span><span class="sxs-lookup"><span data-stu-id="9314e-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="9314e-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="9314e-123">Permission type</span></span>      | <span data-ttu-id="9314e-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9314e-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9314e-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9314e-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="9314e-126">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9314e-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="9314e-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9314e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9314e-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="9314e-128">Not supported.</span></span>    |
|<span data-ttu-id="9314e-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="9314e-129">Application</span></span> | <span data-ttu-id="9314e-130">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9314e-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9314e-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9314e-131">HTTP request</span></span>

<span data-ttu-id="9314e-132">若要删除设备管理提供程序的角色定义，请运行：</span><span class="sxs-lookup"><span data-stu-id="9314e-132">To delete a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="9314e-133">删除目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="9314e-133">To delete a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="9314e-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="9314e-134">Request headers</span></span>

| <span data-ttu-id="9314e-135">名称</span><span class="sxs-lookup"><span data-stu-id="9314e-135">Name</span></span>          | <span data-ttu-id="9314e-136">说明</span><span class="sxs-lookup"><span data-stu-id="9314e-136">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9314e-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="9314e-137">Authorization</span></span> | <span data-ttu-id="9314e-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9314e-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9314e-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="9314e-139">Request body</span></span>

<span data-ttu-id="9314e-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9314e-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9314e-141">响应</span><span class="sxs-lookup"><span data-stu-id="9314e-141">Response</span></span>

<span data-ttu-id="9314e-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9314e-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9314e-144">示例</span><span class="sxs-lookup"><span data-stu-id="9314e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9314e-145">请求</span><span class="sxs-lookup"><span data-stu-id="9314e-145">Request</span></span>

<span data-ttu-id="9314e-146">以下示例删除目录提供程序的 **unifiedRoleDefinition。**</span><span class="sxs-lookup"><span data-stu-id="9314e-146">The following example deletes a **unifiedRoleDefinition** for a directory provider.</span></span>

# <a name="http"></a>[<span data-ttu-id="9314e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9314e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="9314e-148">C#</span><span class="sxs-lookup"><span data-stu-id="9314e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9314e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9314e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9314e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9314e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9314e-151">Java</span><span class="sxs-lookup"><span data-stu-id="9314e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9314e-152">响应</span><span class="sxs-lookup"><span data-stu-id="9314e-152">Response</span></span>

<span data-ttu-id="9314e-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9314e-153">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


