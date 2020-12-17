---
title: 删除 userFlowLanguageConfiguration
description: 从 B2C 用户流中删除 userFlowLanguageConfiguration 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f9396e9522e4f2f6df536e687526b261ce78e6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706314"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="665c5-103">删除 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="665c5-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="665c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="665c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="665c5-105">从[Azure AD B2C](../resources/b2cidentityuserflow.md)用户流中删除[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="665c5-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="665c5-106">**注意：** 无法从 [Azure Active Directory 用户流中删除语言](../resources/b2xidentityuserflow.md)。</span><span class="sxs-lookup"><span data-stu-id="665c5-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="665c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="665c5-107">Permissions</span></span>

<span data-ttu-id="665c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="665c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="665c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="665c5-110">Permission type</span></span>      | <span data-ttu-id="665c5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="665c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="665c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="665c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="665c5-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665c5-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="665c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="665c5-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="665c5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="665c5-115">Not supported.</span></span>|
|<span data-ttu-id="665c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="665c5-116">Application</span></span>|<span data-ttu-id="665c5-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665c5-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="665c5-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="665c5-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="665c5-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="665c5-119">Global administrator</span></span>
* <span data-ttu-id="665c5-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="665c5-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="665c5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="665c5-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="665c5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="665c5-122">Request headers</span></span>

|<span data-ttu-id="665c5-123">名称</span><span class="sxs-lookup"><span data-stu-id="665c5-123">Name</span></span>|<span data-ttu-id="665c5-124">说明</span><span class="sxs-lookup"><span data-stu-id="665c5-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="665c5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="665c5-125">Authorization</span></span>|<span data-ttu-id="665c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="665c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="665c5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="665c5-128">Request body</span></span>

<span data-ttu-id="665c5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="665c5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="665c5-130">响应</span><span class="sxs-lookup"><span data-stu-id="665c5-130">Response</span></span>

<span data-ttu-id="665c5-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="665c5-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="665c5-132">示例</span><span class="sxs-lookup"><span data-stu-id="665c5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="665c5-133">请求</span><span class="sxs-lookup"><span data-stu-id="665c5-133">Request</span></span>

<span data-ttu-id="665c5-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="665c5-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```

### <a name="response"></a><span data-ttu-id="665c5-135">响应</span><span class="sxs-lookup"><span data-stu-id="665c5-135">Response</span></span>

<span data-ttu-id="665c5-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="665c5-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
