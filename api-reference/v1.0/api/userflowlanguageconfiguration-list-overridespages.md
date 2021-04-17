---
title: List overridesPages
description: 从 overridesPages 导航属性获取 userFlowLanguagePage 资源。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5a1836288eda5a52f87bf168833ac4612a9c254e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882982"
---
# <a name="list-overridespages"></a><span data-ttu-id="306f5-103">List overridesPages</span><span class="sxs-lookup"><span data-stu-id="306f5-103">List overridesPages</span></span>

<span data-ttu-id="306f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="306f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="306f5-105">从 overridesPages 导航属性获取 userFlowLanguagePage 资源。</span><span class="sxs-lookup"><span data-stu-id="306f5-105">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="306f5-106">这些页面用于自定义在用户流中的用户旅程期间向用户显示的值。</span><span class="sxs-lookup"><span data-stu-id="306f5-106">These pages are used to customize the values shown to the user during a user journey in a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="306f5-107">权限</span><span class="sxs-lookup"><span data-stu-id="306f5-107">Permissions</span></span>

<span data-ttu-id="306f5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="306f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="306f5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="306f5-110">Permission type</span></span>      | <span data-ttu-id="306f5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="306f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="306f5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="306f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="306f5-113">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="306f5-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="306f5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="306f5-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="306f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="306f5-115">Not supported.</span></span>|
|<span data-ttu-id="306f5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="306f5-116">Application</span></span>|<span data-ttu-id="306f5-117">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="306f5-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="306f5-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="306f5-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="306f5-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="306f5-119">Global administrator</span></span>
* <span data-ttu-id="306f5-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="306f5-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="306f5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="306f5-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages
```

## <a name="request-headers"></a><span data-ttu-id="306f5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="306f5-122">Request headers</span></span>

|<span data-ttu-id="306f5-123">名称</span><span class="sxs-lookup"><span data-stu-id="306f5-123">Name</span></span>|<span data-ttu-id="306f5-124">说明</span><span class="sxs-lookup"><span data-stu-id="306f5-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="306f5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="306f5-125">Authorization</span></span>|<span data-ttu-id="306f5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="306f5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="306f5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="306f5-128">Request body</span></span>

<span data-ttu-id="306f5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="306f5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="306f5-130">响应</span><span class="sxs-lookup"><span data-stu-id="306f5-130">Response</span></span>

<span data-ttu-id="306f5-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="306f5-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="306f5-132">示例</span><span class="sxs-lookup"><span data-stu-id="306f5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="306f5-133">请求</span><span class="sxs-lookup"><span data-stu-id="306f5-133">Request</span></span>

<span data-ttu-id="306f5-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="306f5-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages
```

### <a name="response"></a><span data-ttu-id="306f5-135">响应</span><span class="sxs-lookup"><span data-stu-id="306f5-135">Response</span></span>

<span data-ttu-id="306f5-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="306f5-136">The following is an example of the response.</span></span>

<span data-ttu-id="306f5-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="306f5-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguagePage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "selfasserted1_1"
    }
  ]
}
```
