---
title: 创建 permissionGrantPolicy
description: 创建一个 permissionGrantPolicy 对象，该对象描述可授予权限的条件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 3cfd4a0b13ff3e65be5ffdc8e3486343bef9ce2c
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377145"
---
# <a name="create-permissiongrantpolicy"></a><span data-ttu-id="90ccc-103">创建 permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="90ccc-103">Create permissionGrantPolicy</span></span>

<span data-ttu-id="90ccc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ccc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90ccc-105">创建 [permissionGrantPolicy](../resources/permissiongrantpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="90ccc-105">Creates a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span> <span data-ttu-id="90ccc-106">权限授予策略用于描述可在其上授予权限的条件 (例如，在应用程序同意期间) 。</span><span class="sxs-lookup"><span data-stu-id="90ccc-106">A permission grant policy is used to describe the conditions under which permissions can be granted (for example, during application consent).</span></span>

<span data-ttu-id="90ccc-107">创建权限授予策略后，您可以 [添加包含条件集](permissiongrantpolicy-post-includes.md) 以添加匹配规则， [添加排除条件集](permissiongrantpolicy-post-excludes.md) 以添加排除规则。</span><span class="sxs-lookup"><span data-stu-id="90ccc-107">After creating the permission grant policy, you can [add include condition sets](permissiongrantpolicy-post-includes.md) to add matching rules, and [add exclude condition sets](permissiongrantpolicy-post-excludes.md) to add exclusion rules.</span></span>

## <a name="permissions"></a><span data-ttu-id="90ccc-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="90ccc-108">Permissions</span></span>

<span data-ttu-id="90ccc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90ccc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ccc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="90ccc-111">Permission type</span></span>      | <span data-ttu-id="90ccc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90ccc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90ccc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90ccc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="90ccc-114">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="90ccc-114">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="90ccc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90ccc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90ccc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90ccc-116">Not supported.</span></span>    |
|<span data-ttu-id="90ccc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="90ccc-117">Application</span></span> | <span data-ttu-id="90ccc-118">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="90ccc-118">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90ccc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90ccc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /policies/permissionGrantPolicies
```

## <a name="request-headers"></a><span data-ttu-id="90ccc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="90ccc-120">Request headers</span></span>

| <span data-ttu-id="90ccc-121">名称</span><span class="sxs-lookup"><span data-stu-id="90ccc-121">Name</span></span>       | <span data-ttu-id="90ccc-122">说明</span><span class="sxs-lookup"><span data-stu-id="90ccc-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="90ccc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90ccc-123">Authorization</span></span> | <span data-ttu-id="90ccc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90ccc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90ccc-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="90ccc-126">Content-type</span></span> | <span data-ttu-id="90ccc-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="90ccc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90ccc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="90ccc-129">Request body</span></span>

<span data-ttu-id="90ccc-130">在请求正文中，提供 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90ccc-130">In the request body, supply a JSON representation of an [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="90ccc-131">响应</span><span class="sxs-lookup"><span data-stu-id="90ccc-131">Response</span></span>

<span data-ttu-id="90ccc-132">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90ccc-132">If successful, this method returns a `201 Created` response code and a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90ccc-133">示例</span><span class="sxs-lookup"><span data-stu-id="90ccc-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90ccc-134">请求</span><span class="sxs-lookup"><span data-stu-id="90ccc-134">Request</span></span>

<span data-ttu-id="90ccc-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="90ccc-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "create_permissiongrantpolicy"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies
Content-Type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```

### <a name="response"></a><span data-ttu-id="90ccc-136">响应</span><span class="sxs-lookup"><span data-stu-id="90ccc-136">Response</span></span>

<span data-ttu-id="90ccc-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="90ccc-137">The following is an example of the response.</span></span>

> <span data-ttu-id="90ccc-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="90ccc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
