---
title: 删除 userFlowLanguagePage
description: 删除 userFlowLanguagePage 对象中的值。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 22efb148458c20709c58bde0ea9b198566912a41
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706306"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="56185-103">删除 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="56185-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="56185-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56185-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56185-105">删除 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 中的值。</span><span class="sxs-lookup"><span data-stu-id="56185-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="56185-106">只能删除 overridesPage 中的值，overridesPage 用于在用户流定义的用户旅程中自定义向用户显示的值。</span><span class="sxs-lookup"><span data-stu-id="56185-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="56185-107">权限</span><span class="sxs-lookup"><span data-stu-id="56185-107">Permissions</span></span>

<span data-ttu-id="56185-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56185-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56185-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="56185-110">Permission type</span></span>      | <span data-ttu-id="56185-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56185-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56185-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56185-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56185-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56185-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="56185-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56185-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="56185-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="56185-115">Not supported.</span></span>|
|<span data-ttu-id="56185-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="56185-116">Application</span></span>|<span data-ttu-id="56185-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56185-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="56185-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="56185-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="56185-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="56185-119">Global administrator</span></span>
* <span data-ttu-id="56185-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="56185-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="56185-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56185-121">HTTP request</span></span>

<span data-ttu-id="56185-122">若要引用对象中的内容，必须使用 `$value` 。</span><span class="sxs-lookup"><span data-stu-id="56185-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="56185-123">这将返回对象中的内容，并允许你直接引用它。</span><span class="sxs-lookup"><span data-stu-id="56185-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/$value
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="56185-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="56185-124">Request headers</span></span>

|<span data-ttu-id="56185-125">名称</span><span class="sxs-lookup"><span data-stu-id="56185-125">Name</span></span>|<span data-ttu-id="56185-126">说明</span><span class="sxs-lookup"><span data-stu-id="56185-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="56185-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="56185-127">Authorization</span></span>|<span data-ttu-id="56185-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56185-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56185-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="56185-130">Request body</span></span>

<span data-ttu-id="56185-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56185-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56185-132">响应</span><span class="sxs-lookup"><span data-stu-id="56185-132">Response</span></span>

<span data-ttu-id="56185-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="56185-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="56185-134">示例</span><span class="sxs-lookup"><span data-stu-id="56185-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56185-135">请求</span><span class="sxs-lookup"><span data-stu-id="56185-135">Request</span></span>

<span data-ttu-id="56185-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56185-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
```

### <a name="response"></a><span data-ttu-id="56185-137">响应</span><span class="sxs-lookup"><span data-stu-id="56185-137">Response</span></span>

<span data-ttu-id="56185-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56185-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
