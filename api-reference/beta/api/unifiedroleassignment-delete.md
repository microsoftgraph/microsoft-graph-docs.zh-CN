---
title: 删除 unifiedRoleAssignment
description: 删除 unifiedRoleAssignment 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9540a1104e2729c65c716a4f64010119b3941ed5
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437781"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="fefe3-103">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fefe3-103">Delete unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fefe3-104">删除[unifiedRoleAssignment](../resources/unifiedRoleAssignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fefe3-104">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fefe3-105">权限</span><span class="sxs-lookup"><span data-stu-id="fefe3-105">Permissions</span></span>

<span data-ttu-id="fefe3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fefe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fefe3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fefe3-108">Permission type</span></span>                        | <span data-ttu-id="fefe3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fefe3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fefe3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fefe3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fefe3-111">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="fefe3-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="fefe3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fefe3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fefe3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fefe3-113">Not supported.</span></span> |
| <span data-ttu-id="fefe3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fefe3-114">Application</span></span>                            | <span data-ttu-id="fefe3-115">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="fefe3-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="fefe3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fefe3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fefe3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fefe3-117">Request headers</span></span>

| <span data-ttu-id="fefe3-118">名称</span><span class="sxs-lookup"><span data-stu-id="fefe3-118">Name</span></span>          | <span data-ttu-id="fefe3-119">说明</span><span class="sxs-lookup"><span data-stu-id="fefe3-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fefe3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fefe3-120">Authorization</span></span> | <span data-ttu-id="fefe3-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="fefe3-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fefe3-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="fefe3-122">Request body</span></span>

<span data-ttu-id="fefe3-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fefe3-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fefe3-124">响应</span><span class="sxs-lookup"><span data-stu-id="fefe3-124">Response</span></span>

<span data-ttu-id="fefe3-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fefe3-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fefe3-127">示例</span><span class="sxs-lookup"><span data-stu-id="fefe3-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="fefe3-128">请求</span><span class="sxs-lookup"><span data-stu-id="fefe3-128">Request</span></span>

<span data-ttu-id="fefe3-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fefe3-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

### <a name="response"></a><span data-ttu-id="fefe3-130">响应</span><span class="sxs-lookup"><span data-stu-id="fefe3-130">Response</span></span>

<span data-ttu-id="fefe3-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fefe3-131">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
