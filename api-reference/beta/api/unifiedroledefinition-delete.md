---
title: 删除 unifiedRoleDefinition
description: 删除 unifiedRoleDefinition 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e9f2d549cef274a536575a2671e454198dbb9f5f
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709498"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="1a2ad-103">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1a2ad-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="1a2ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a2ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a2ad-105">删除 RBAC 提供程序的 [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="1a2ad-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="1a2ad-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="1a2ad-107">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="1a2ad-107">device management (Intune)</span></span>
- <span data-ttu-id="1a2ad-108">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="1a2ad-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="1a2ad-109">云电脑 RBAC 提供商当前仅支持[列表和](rbacapplication-list-roledefinitions.md)[获取](unifiedroledefinition-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a2ad-110">权限</span><span class="sxs-lookup"><span data-stu-id="1a2ad-110">Permissions</span></span>

<span data-ttu-id="1a2ad-111">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="1a2ad-112">若要了解详细信息，包括在选择更多特权之前的[注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，请在“[权限](/graph/permissions-reference)”中搜索以下权限。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="1a2ad-113">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="1a2ad-113">Supported provider</span></span>      | <span data-ttu-id="1a2ad-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a2ad-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="1a2ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a2ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a2ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a2ad-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="1a2ad-117">设备管理</span><span class="sxs-lookup"><span data-stu-id="1a2ad-117">Device management</span></span> | <span data-ttu-id="1a2ad-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2ad-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="1a2ad-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-119">Not supported.</span></span> | <span data-ttu-id="1a2ad-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2ad-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="1a2ad-121">目录</span><span class="sxs-lookup"><span data-stu-id="1a2ad-121">Directory</span></span> | <span data-ttu-id="1a2ad-122">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a2ad-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="1a2ad-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-123">Not supported.</span></span>| <span data-ttu-id="1a2ad-124">RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2ad-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a2ad-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a2ad-125">HTTP request</span></span>

<span data-ttu-id="1a2ad-126">若要删除设备管理提供程序的角色定义，请运行：</span><span class="sxs-lookup"><span data-stu-id="1a2ad-126">To delete a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="1a2ad-127">删除目录提供程序的角色定义：</span><span class="sxs-lookup"><span data-stu-id="1a2ad-127">To delete a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="1a2ad-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a2ad-128">Request headers</span></span>

| <span data-ttu-id="1a2ad-129">名称</span><span class="sxs-lookup"><span data-stu-id="1a2ad-129">Name</span></span>          | <span data-ttu-id="1a2ad-130">说明</span><span class="sxs-lookup"><span data-stu-id="1a2ad-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1a2ad-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a2ad-131">Authorization</span></span> | <span data-ttu-id="1a2ad-132">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1a2ad-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a2ad-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a2ad-133">Request body</span></span>

<span data-ttu-id="1a2ad-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a2ad-135">响应</span><span class="sxs-lookup"><span data-stu-id="1a2ad-135">Response</span></span>

<span data-ttu-id="1a2ad-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a2ad-138">示例</span><span class="sxs-lookup"><span data-stu-id="1a2ad-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a2ad-139">请求</span><span class="sxs-lookup"><span data-stu-id="1a2ad-139">Request</span></span>

<span data-ttu-id="1a2ad-140">以下示例删除目录提供程序的 **unifiedRoleDefinition。**</span><span class="sxs-lookup"><span data-stu-id="1a2ad-140">The following example deletes a **unifiedRoleDefinition** for a directory provider.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a2ad-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a2ad-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="1a2ad-142">C#</span><span class="sxs-lookup"><span data-stu-id="1a2ad-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a2ad-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a2ad-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a2ad-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a2ad-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a2ad-145">Java</span><span class="sxs-lookup"><span data-stu-id="1a2ad-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a2ad-146">响应</span><span class="sxs-lookup"><span data-stu-id="1a2ad-146">Response</span></span>

<span data-ttu-id="1a2ad-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a2ad-147">The following is an example of the response.</span></span>

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


