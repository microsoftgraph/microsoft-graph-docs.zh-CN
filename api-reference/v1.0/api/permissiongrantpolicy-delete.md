---
title: 删除 permissionGrantPolicy
description: 删除 permissionGrantPolicy 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 5c977da45c2e640e041dc37c8be2fb17c49a8424
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377231"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="000a2-103">删除 permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="000a2-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="000a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="000a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="000a2-105">删除 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="000a2-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="000a2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="000a2-106">Permissions</span></span>

<span data-ttu-id="000a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="000a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="000a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="000a2-109">Permission type</span></span>                        | <span data-ttu-id="000a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="000a2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="000a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="000a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="000a2-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="000a2-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="000a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="000a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="000a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="000a2-114">Not supported.</span></span> |
| <span data-ttu-id="000a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="000a2-115">Application</span></span>                            | <span data-ttu-id="000a2-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="000a2-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="000a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="000a2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="000a2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="000a2-118">Request headers</span></span>

| <span data-ttu-id="000a2-119">名称</span><span class="sxs-lookup"><span data-stu-id="000a2-119">Name</span></span>           | <span data-ttu-id="000a2-120">说明</span><span class="sxs-lookup"><span data-stu-id="000a2-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="000a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="000a2-121">Authorization</span></span>  | <span data-ttu-id="000a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="000a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="000a2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="000a2-124">Request body</span></span>

<span data-ttu-id="000a2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="000a2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="000a2-126">响应</span><span class="sxs-lookup"><span data-stu-id="000a2-126">Response</span></span>

<span data-ttu-id="000a2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="000a2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="000a2-129">示例</span><span class="sxs-lookup"><span data-stu-id="000a2-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="000a2-130">请求</span><span class="sxs-lookup"><span data-stu-id="000a2-130">Request</span></span>

<span data-ttu-id="000a2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="000a2-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy
```

### <a name="response"></a><span data-ttu-id="000a2-132">响应</span><span class="sxs-lookup"><span data-stu-id="000a2-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
