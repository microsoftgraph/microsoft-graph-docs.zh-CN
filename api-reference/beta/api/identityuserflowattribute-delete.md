---
title: 删除 identityUserFlowAttribute
description: 删除 identityUserFlowAttribute。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6912769c140a95054c30c67defc4068a5a8b4e43
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904116"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="2a675-103">删除 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="2a675-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="2a675-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a675-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a675-105">删除 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="2a675-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="2a675-106">仅可删除自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="2a675-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a675-107">权限</span><span class="sxs-lookup"><span data-stu-id="2a675-107">Permissions</span></span>

<span data-ttu-id="2a675-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a675-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a675-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a675-110">Permission type</span></span>      | <span data-ttu-id="2a675-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a675-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a675-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a675-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a675-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a675-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2a675-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a675-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2a675-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a675-115">Not supported.</span></span>|
|<span data-ttu-id="2a675-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a675-116">Application</span></span>|<span data-ttu-id="2a675-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a675-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="2a675-118">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="2a675-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2a675-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2a675-119">Global administrator</span></span>
* <span data-ttu-id="2a675-120">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="2a675-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2a675-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a675-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2a675-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a675-122">Request headers</span></span>

|<span data-ttu-id="2a675-123">名称</span><span class="sxs-lookup"><span data-stu-id="2a675-123">Name</span></span>|<span data-ttu-id="2a675-124">说明</span><span class="sxs-lookup"><span data-stu-id="2a675-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2a675-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a675-125">Authorization</span></span>|<span data-ttu-id="2a675-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a675-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a675-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a675-128">Request body</span></span>

<span data-ttu-id="2a675-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a675-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a675-130">响应</span><span class="sxs-lookup"><span data-stu-id="2a675-130">Response</span></span>

<span data-ttu-id="2a675-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2a675-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a675-132">示例</span><span class="sxs-lookup"><span data-stu-id="2a675-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a675-133">请求</span><span class="sxs-lookup"><span data-stu-id="2a675-133">Request</span></span>

<span data-ttu-id="2a675-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a675-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a675-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a675-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="2a675-136">C#</span><span class="sxs-lookup"><span data-stu-id="2a675-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a675-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a675-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a675-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a675-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a675-139">响应</span><span class="sxs-lookup"><span data-stu-id="2a675-139">Response</span></span>

<span data-ttu-id="2a675-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a675-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
