---
title: 删除 unifiedRoleAssignmentMultiple
description: 删除 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 18b164b09ad3b06f02b3be0890aeada32946b48b
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160347"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="fce24-103">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fce24-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="fce24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fce24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fce24-105">删除[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fce24-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="fce24-106">这适用于支持多个主体和作用域的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="fce24-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="fce24-107">Microsoft Intune 是这样一个应用程序。</span><span class="sxs-lookup"><span data-stu-id="fce24-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fce24-108">权限</span><span class="sxs-lookup"><span data-stu-id="fce24-108">Permissions</span></span>

<span data-ttu-id="fce24-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fce24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fce24-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fce24-111">Permission type</span></span> | <span data-ttu-id="fce24-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fce24-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="fce24-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fce24-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fce24-114">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="fce24-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="fce24-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fce24-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fce24-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fce24-116">Not supported.</span></span> |
| <span data-ttu-id="fce24-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fce24-117">Application</span></span> | <span data-ttu-id="fce24-118">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="fce24-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="fce24-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fce24-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fce24-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fce24-120">Request headers</span></span>

| <span data-ttu-id="fce24-121">名称</span><span class="sxs-lookup"><span data-stu-id="fce24-121">Name</span></span> | <span data-ttu-id="fce24-122">说明</span><span class="sxs-lookup"><span data-stu-id="fce24-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="fce24-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fce24-123">Authorization</span></span> | <span data-ttu-id="fce24-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="fce24-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fce24-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fce24-125">Request body</span></span>

<span data-ttu-id="fce24-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fce24-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fce24-127">响应</span><span class="sxs-lookup"><span data-stu-id="fce24-127">Response</span></span>

<span data-ttu-id="fce24-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fce24-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fce24-130">示例</span><span class="sxs-lookup"><span data-stu-id="fce24-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fce24-131">请求</span><span class="sxs-lookup"><span data-stu-id="fce24-131">Request</span></span>

<span data-ttu-id="fce24-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fce24-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

### <a name="response"></a><span data-ttu-id="fce24-133">响应</span><span class="sxs-lookup"><span data-stu-id="fce24-133">Response</span></span>

<span data-ttu-id="fce24-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fce24-134">The following is an example of the response.</span></span>

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