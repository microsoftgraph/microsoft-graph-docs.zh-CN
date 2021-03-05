---
title: 获取 authorizationPolicy
description: 检索 authorizationPolicy 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7ffb4e245e9a24f5ed33576dbd414891ee5d28ac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434914"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="943c4-103">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="943c4-103">Get authorizationPolicy</span></span>

<span data-ttu-id="943c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="943c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="943c4-105">检索 [authorizationPolicy 对象](../resources/authorizationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="943c4-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="943c4-106">权限</span><span class="sxs-lookup"><span data-stu-id="943c4-106">Permissions</span></span>

<span data-ttu-id="943c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="943c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="943c4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="943c4-109">Permission type</span></span>                        | <span data-ttu-id="943c4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="943c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="943c4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="943c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="943c4-112">Policy.Read.All、Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="943c4-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="943c4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="943c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="943c4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="943c4-114">Not supported.</span></span> |
| <span data-ttu-id="943c4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="943c4-115">Application</span></span>                            | <span data-ttu-id="943c4-116">Policy.Read.All、Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="943c4-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="943c4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="943c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="943c4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="943c4-118">Request headers</span></span>

| <span data-ttu-id="943c4-119">名称</span><span class="sxs-lookup"><span data-stu-id="943c4-119">Name</span></span>      |<span data-ttu-id="943c4-120">说明</span><span class="sxs-lookup"><span data-stu-id="943c4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="943c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="943c4-121">Authorization</span></span> | <span data-ttu-id="943c4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="943c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="943c4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="943c4-124">Request body</span></span>

<span data-ttu-id="943c4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="943c4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="943c4-126">响应</span><span class="sxs-lookup"><span data-stu-id="943c4-126">Response</span></span>

<span data-ttu-id="943c4-127">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和单个 [authorizationPolicy](../resources/authorizationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="943c4-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="943c4-128">示例</span><span class="sxs-lookup"><span data-stu-id="943c4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="943c4-129">请求</span><span class="sxs-lookup"><span data-stu-id="943c4-129">Request</span></span>

<span data-ttu-id="943c4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="943c4-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="943c4-131">响应</span><span class="sxs-lookup"><span data-stu-id="943c4-131">Response</span></span>

<span data-ttu-id="943c4-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="943c4-132">The following is an example of the response.</span></span>

> <span data-ttu-id="943c4-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="943c4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authorizationPolicy/$entity",
    "id": "authorizationPolicy",
    "allowInvitesFrom": "everyone",
    "allowedToSignUpEmailBasedSubscriptions": true,
    "allowedToUseSSPR": true,
    "allowEmailVerifiedUsersToJoinOrganization": true,
    "blockMsolPowerShell": null,
    "displayName": "Authorization Policy",
    "description": "Used to manage authorization related settings across the company.",
    "defaultUserRolePermissions": {
        "allowedToCreateApps": true,
        "allowedToCreateSecurityGroups": true,
        "allowedToReadOtherUsers": true,
        "permissionGrantPoliciesAssigned": [
            "just-user-read"
        ]
    }
}
```
