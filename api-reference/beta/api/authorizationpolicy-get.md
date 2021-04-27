---
title: 获取 authorizationPolicy
description: 检索 authorizationPolicy 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ca66332d7461dfe4e2fc298fffab9ed0cff6e795
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047950"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="811b2-103">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="811b2-103">Get authorizationPolicy</span></span>

<span data-ttu-id="811b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="811b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="811b2-105">检索 [authorizationPolicy 对象](../resources/authorizationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="811b2-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="811b2-106">权限</span><span class="sxs-lookup"><span data-stu-id="811b2-106">Permissions</span></span>

<span data-ttu-id="811b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="811b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="811b2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="811b2-109">Permission type</span></span>                        | <span data-ttu-id="811b2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="811b2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="811b2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="811b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="811b2-112">Policy.Read.All、Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="811b2-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="811b2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="811b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="811b2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="811b2-114">Not supported.</span></span> |
| <span data-ttu-id="811b2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="811b2-115">Application</span></span>                            | <span data-ttu-id="811b2-116">Policy.Read.All、Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="811b2-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="811b2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="811b2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="811b2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="811b2-118">Request headers</span></span>

| <span data-ttu-id="811b2-119">名称</span><span class="sxs-lookup"><span data-stu-id="811b2-119">Name</span></span>      |<span data-ttu-id="811b2-120">说明</span><span class="sxs-lookup"><span data-stu-id="811b2-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="811b2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="811b2-121">Authorization</span></span> | <span data-ttu-id="811b2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="811b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="811b2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="811b2-124">Request body</span></span>

<span data-ttu-id="811b2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="811b2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="811b2-126">响应</span><span class="sxs-lookup"><span data-stu-id="811b2-126">Response</span></span>

<span data-ttu-id="811b2-127">如果成功，此方法在响应正文中返回 响应代码和单个 `200 OK` [authorizationPolicy](../resources/authorizationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="811b2-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="811b2-128">示例</span><span class="sxs-lookup"><span data-stu-id="811b2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="811b2-129">请求</span><span class="sxs-lookup"><span data-stu-id="811b2-129">Request</span></span>

<span data-ttu-id="811b2-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="811b2-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="811b2-131">响应</span><span class="sxs-lookup"><span data-stu-id="811b2-131">Response</span></span>

<span data-ttu-id="811b2-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="811b2-132">The following is an example of the response.</span></span>

> <span data-ttu-id="811b2-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="811b2-133">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authorizationPolicy/$entity",
    "id": "authorizationPolicy",
    "displayName": "Authorization Policy",
    "description": "Used to manage authorization related settings across the company.",
    "enabledPreviewFeatures": [],
    "guestUserRoleId": "10dae51f-b6af-4016-8d66-8c2a99b929b3",
    "blockMsolPowerShell": ""
    "defaultUserRolePermissions": {
        "allowedToCreateApps": true,
        "allowedToCreateSecurityGroups": false,
        "allowedToReadOtherUsers": true
    }
    "allowedToSignUpEmailBasedSubscriptions": false,
    "allowedToUseSSPR": true,
    "allowEmailVerifiedUsersToJoinOrganization": true,
    "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
        "managePermissionGrantsForSelf.microsoft-user-default-low"
    ]
}
```


