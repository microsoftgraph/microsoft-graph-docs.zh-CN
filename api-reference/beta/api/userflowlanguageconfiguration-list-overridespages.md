---
title: List overridesPages
description: 从 overridesPages 导航属性获取 userFlowLanguagePage 资源。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 24cbab257c2ff0c49a97b4e8260bdc4d0d1cb0f7
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626108"
---
# <a name="list-overridespages"></a><span data-ttu-id="4ae77-103">List overridesPages</span><span class="sxs-lookup"><span data-stu-id="4ae77-103">List overridesPages</span></span>

<span data-ttu-id="4ae77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ae77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ae77-105">从 overridesPages 导航属性获取 userFlowLanguagePage 资源。</span><span class="sxs-lookup"><span data-stu-id="4ae77-105">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="4ae77-106">这些页面用于自定义在用户流中的用户旅程期间向用户显示的值。</span><span class="sxs-lookup"><span data-stu-id="4ae77-106">These pages are used to customize the values shown to the user during a user journey in a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ae77-107">权限</span><span class="sxs-lookup"><span data-stu-id="4ae77-107">Permissions</span></span>

<span data-ttu-id="4ae77-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ae77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae77-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ae77-110">Permission type</span></span>      | <span data-ttu-id="4ae77-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ae77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ae77-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ae77-113">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae77-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4ae77-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae77-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4ae77-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae77-115">Not supported.</span></span>|
|<span data-ttu-id="4ae77-116">Application</span><span class="sxs-lookup"><span data-stu-id="4ae77-116">Application</span></span>|<span data-ttu-id="4ae77-117">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae77-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4ae77-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4ae77-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4ae77-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4ae77-119">Global administrator</span></span>
* <span data-ttu-id="4ae77-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="4ae77-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4ae77-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ae77-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/overridesPages
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages
```

## <a name="request-headers"></a><span data-ttu-id="4ae77-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ae77-122">Request headers</span></span>

|<span data-ttu-id="4ae77-123">名称</span><span class="sxs-lookup"><span data-stu-id="4ae77-123">Name</span></span>|<span data-ttu-id="4ae77-124">说明</span><span class="sxs-lookup"><span data-stu-id="4ae77-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ae77-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ae77-125">Authorization</span></span>|<span data-ttu-id="4ae77-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ae77-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae77-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ae77-128">Request body</span></span>

<span data-ttu-id="4ae77-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ae77-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ae77-130">响应</span><span class="sxs-lookup"><span data-stu-id="4ae77-130">Response</span></span>

<span data-ttu-id="4ae77-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ae77-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ae77-132">示例</span><span class="sxs-lookup"><span data-stu-id="4ae77-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ae77-133">请求</span><span class="sxs-lookup"><span data-stu-id="4ae77-133">Request</span></span>

<span data-ttu-id="4ae77-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ae77-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages
```


### <a name="response"></a><span data-ttu-id="4ae77-135">响应</span><span class="sxs-lookup"><span data-stu-id="4ae77-135">Response</span></span>

<span data-ttu-id="4ae77-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ae77-136">The following is an example of the response.</span></span>

<span data-ttu-id="4ae77-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ae77-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "idpselections"
    },
    {
      "id": "phonefactor"
    }
  ]
}
```
