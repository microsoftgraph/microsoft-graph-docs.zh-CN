---
title: 删除 userFlowLanguagePage
description: 删除 userFlowLanguagePage 对象中的值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f9c1ba04d2c3cfdf60e4309d0a274388639b83a7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666606"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="50d92-103">删除 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="50d92-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="50d92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50d92-105">删除 [userFlowLanguagePage 对象中的](../resources/userflowlanguagepage.md) 值。</span><span class="sxs-lookup"><span data-stu-id="50d92-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="50d92-106">只能删除 overridesPage 中的值，这些值用于自定义在用户流定义的用户旅程期间向用户显示的值。</span><span class="sxs-lookup"><span data-stu-id="50d92-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="50d92-107">权限</span><span class="sxs-lookup"><span data-stu-id="50d92-107">Permissions</span></span>

<span data-ttu-id="50d92-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50d92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d92-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="50d92-110">Permission type</span></span>      | <span data-ttu-id="50d92-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50d92-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50d92-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50d92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50d92-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d92-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="50d92-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50d92-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="50d92-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="50d92-115">Not supported.</span></span>|
|<span data-ttu-id="50d92-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="50d92-116">Application</span></span>|<span data-ttu-id="50d92-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d92-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="50d92-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="50d92-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="50d92-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="50d92-119">Global administrator</span></span>
* <span data-ttu-id="50d92-120">外部标识用户Flow管理员</span><span class="sxs-lookup"><span data-stu-id="50d92-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="50d92-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50d92-121">HTTP request</span></span>

<span data-ttu-id="50d92-122">若要引用对象中的内容，必须使用 `$value` 。</span><span class="sxs-lookup"><span data-stu-id="50d92-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="50d92-123">这将返回 对象中的内容，并允许你直接引用它。</span><span class="sxs-lookup"><span data-stu-id="50d92-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="50d92-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="50d92-124">Request headers</span></span>

|<span data-ttu-id="50d92-125">名称</span><span class="sxs-lookup"><span data-stu-id="50d92-125">Name</span></span>|<span data-ttu-id="50d92-126">说明</span><span class="sxs-lookup"><span data-stu-id="50d92-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="50d92-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="50d92-127">Authorization</span></span>|<span data-ttu-id="50d92-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50d92-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50d92-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="50d92-130">Request body</span></span>

<span data-ttu-id="50d92-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50d92-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50d92-132">响应</span><span class="sxs-lookup"><span data-stu-id="50d92-132">Response</span></span>

<span data-ttu-id="50d92-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="50d92-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="50d92-134">示例</span><span class="sxs-lookup"><span data-stu-id="50d92-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50d92-135">请求</span><span class="sxs-lookup"><span data-stu-id="50d92-135">Request</span></span>

<span data-ttu-id="50d92-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="50d92-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50d92-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="50d92-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value
```
# <a name="c"></a>[<span data-ttu-id="50d92-138">C#</span><span class="sxs-lookup"><span data-stu-id="50d92-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50d92-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50d92-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50d92-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50d92-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50d92-141">Java</span><span class="sxs-lookup"><span data-stu-id="50d92-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50d92-142">响应</span><span class="sxs-lookup"><span data-stu-id="50d92-142">Response</span></span>

<span data-ttu-id="50d92-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="50d92-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
