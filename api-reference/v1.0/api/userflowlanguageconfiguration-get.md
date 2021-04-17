---
title: 获取 userFlowLanguageConfiguration
description: 读取 userFlowLanguageConfiguration 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 054ed16948c86b872ee82572c770425e1c7b457b
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882816"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="e08b6-103">获取 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="e08b6-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="e08b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e08b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e08b6-105">读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e08b6-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="e08b6-106">这些对象表示用户流中可用的语言。</span><span class="sxs-lookup"><span data-stu-id="e08b6-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="e08b6-107">**注意：** 默认情况下，在 Azure Active Directory 用户流 [中启用语言自定义](../resources/b2xidentityuserflow.md)。</span><span class="sxs-lookup"><span data-stu-id="e08b6-107">**Note:** Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e08b6-108">权限</span><span class="sxs-lookup"><span data-stu-id="e08b6-108">Permissions</span></span>

<span data-ttu-id="e08b6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e08b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e08b6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e08b6-111">Permission type</span></span>      | <span data-ttu-id="e08b6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e08b6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e08b6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e08b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e08b6-114">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e08b6-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e08b6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e08b6-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e08b6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e08b6-116">Not supported.</span></span>|
|<span data-ttu-id="e08b6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e08b6-117">Application</span></span>|<span data-ttu-id="e08b6-118">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e08b6-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e08b6-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="e08b6-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e08b6-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e08b6-120">Global administrator</span></span>
* <span data-ttu-id="e08b6-121">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="e08b6-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e08b6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e08b6-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e08b6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e08b6-123">Request headers</span></span>

|<span data-ttu-id="e08b6-124">名称</span><span class="sxs-lookup"><span data-stu-id="e08b6-124">Name</span></span>|<span data-ttu-id="e08b6-125">说明</span><span class="sxs-lookup"><span data-stu-id="e08b6-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e08b6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e08b6-126">Authorization</span></span>|<span data-ttu-id="e08b6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e08b6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e08b6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e08b6-129">Request body</span></span>

<span data-ttu-id="e08b6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e08b6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e08b6-131">响应</span><span class="sxs-lookup"><span data-stu-id="e08b6-131">Response</span></span>

<span data-ttu-id="e08b6-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e08b6-132">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e08b6-133">示例</span><span class="sxs-lookup"><span data-stu-id="e08b6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e08b6-134">请求</span><span class="sxs-lookup"><span data-stu-id="e08b6-134">Request</span></span>

<span data-ttu-id="e08b6-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e08b6-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en
```

### <a name="response"></a><span data-ttu-id="e08b6-136">响应</span><span class="sxs-lookup"><span data-stu-id="e08b6-136">Response</span></span>

<span data-ttu-id="e08b6-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e08b6-137">The following is an example of the response.</span></span>

<span data-ttu-id="e08b6-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e08b6-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_Partner')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
