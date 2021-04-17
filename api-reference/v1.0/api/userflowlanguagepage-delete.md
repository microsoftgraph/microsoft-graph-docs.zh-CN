---
title: 删除 userFlowLanguagePage
description: 删除 userFlowLanguagePage 对象中的值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 791c43817d9a8f8e8369e4d0d8adf5eb0a75580a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882979"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="ddac9-103">删除 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="ddac9-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="ddac9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddac9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddac9-105">删除 [userFlowLanguagePage 对象中的](../resources/userflowlanguagepage.md) 值。</span><span class="sxs-lookup"><span data-stu-id="ddac9-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="ddac9-106">只能删除 overridesPage 中的值，这些值用于自定义在用户流定义的用户旅程期间向用户显示的值。</span><span class="sxs-lookup"><span data-stu-id="ddac9-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddac9-107">权限</span><span class="sxs-lookup"><span data-stu-id="ddac9-107">Permissions</span></span>

<span data-ttu-id="ddac9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddac9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddac9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddac9-110">Permission type</span></span>      | <span data-ttu-id="ddac9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddac9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddac9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddac9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddac9-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddac9-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ddac9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddac9-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ddac9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddac9-115">Not supported.</span></span>|
|<span data-ttu-id="ddac9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddac9-116">Application</span></span>|<span data-ttu-id="ddac9-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddac9-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ddac9-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="ddac9-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ddac9-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ddac9-119">Global administrator</span></span>
* <span data-ttu-id="ddac9-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="ddac9-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ddac9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddac9-121">HTTP request</span></span>

<span data-ttu-id="ddac9-122">若要引用对象中的内容，必须使用 `$value` 。</span><span class="sxs-lookup"><span data-stu-id="ddac9-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="ddac9-123">这将返回 对象中的内容，并允许你直接引用它。</span><span class="sxs-lookup"><span data-stu-id="ddac9-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="ddac9-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddac9-124">Request headers</span></span>

|<span data-ttu-id="ddac9-125">名称</span><span class="sxs-lookup"><span data-stu-id="ddac9-125">Name</span></span>|<span data-ttu-id="ddac9-126">说明</span><span class="sxs-lookup"><span data-stu-id="ddac9-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ddac9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddac9-127">Authorization</span></span>|<span data-ttu-id="ddac9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddac9-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddac9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddac9-130">Request body</span></span>

<span data-ttu-id="ddac9-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddac9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddac9-132">响应</span><span class="sxs-lookup"><span data-stu-id="ddac9-132">Response</span></span>

<span data-ttu-id="ddac9-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ddac9-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ddac9-134">示例</span><span class="sxs-lookup"><span data-stu-id="ddac9-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddac9-135">请求</span><span class="sxs-lookup"><span data-stu-id="ddac9-135">Request</span></span>

<span data-ttu-id="ddac9-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ddac9-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value
```

### <a name="response"></a><span data-ttu-id="ddac9-137">响应</span><span class="sxs-lookup"><span data-stu-id="ddac9-137">Response</span></span>

<span data-ttu-id="ddac9-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ddac9-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
