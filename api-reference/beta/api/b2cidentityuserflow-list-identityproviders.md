---
title: '列出 b2cIdentityUserFlow 中已弃 (identityProviders) '
description: '列出 b2cIdentityUserFlow 中所有 identityProviders。  (已弃) '
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7e83384f009c273197ea8bd8b978e27dd75263a8
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400976"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="aa3e9-104">列出 b2cIdentityUserFlow 中已弃 (identityProviders) </span><span class="sxs-lookup"><span data-stu-id="aa3e9-104">List all identityProviders in a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="aa3e9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa3e9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="aa3e9-106">获取 [b2cIdentityUserFlow 对象中的标识](../resources/b2cidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-106">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa3e9-107">权限</span><span class="sxs-lookup"><span data-stu-id="aa3e9-107">Permissions</span></span>

<span data-ttu-id="aa3e9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa3e9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa3e9-110">Permission type</span></span>      | <span data-ttu-id="aa3e9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa3e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa3e9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa3e9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa3e9-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa3e9-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="aa3e9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa3e9-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="aa3e9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-115">Not supported.</span></span>|
|<span data-ttu-id="aa3e9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa3e9-116">Application</span></span>| <span data-ttu-id="aa3e9-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa3e9-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="aa3e9-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="aa3e9-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="aa3e9-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="aa3e9-119">Global administrator</span></span>
* <span data-ttu-id="aa3e9-120">外部标识用户Flow管理员</span><span class="sxs-lookup"><span data-stu-id="aa3e9-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="aa3e9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa3e9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="aa3e9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa3e9-122">Request headers</span></span>

|<span data-ttu-id="aa3e9-123">名称</span><span class="sxs-lookup"><span data-stu-id="aa3e9-123">Name</span></span>|<span data-ttu-id="aa3e9-124">说明</span><span class="sxs-lookup"><span data-stu-id="aa3e9-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="aa3e9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa3e9-125">Authorization</span></span>|<span data-ttu-id="aa3e9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa3e9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa3e9-128">Request body</span></span>

<span data-ttu-id="aa3e9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa3e9-130">响应</span><span class="sxs-lookup"><span data-stu-id="aa3e9-130">Response</span></span>

<span data-ttu-id="aa3e9-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityProviders](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-131">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa3e9-132">示例</span><span class="sxs-lookup"><span data-stu-id="aa3e9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa3e9-133">请求</span><span class="sxs-lookup"><span data-stu-id="aa3e9-133">Request</span></span>

<span data-ttu-id="aa3e9-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```

### <a name="response"></a><span data-ttu-id="aa3e9-135">响应</span><span class="sxs-lookup"><span data-stu-id="aa3e9-135">Response</span></span>

<span data-ttu-id="aa3e9-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa3e9-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "*****"
        },
        {
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}
```
