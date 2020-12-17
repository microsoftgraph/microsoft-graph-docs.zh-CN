---
title: 获取 userFlowLanguageConfiguration
description: 读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d25533822a5f67cdfc98564a41e7f53b3be98208
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706290"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="a40b1-103">获取 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="a40b1-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="a40b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a40b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a40b1-105">读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a40b1-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="a40b1-106">这些对象表示用户流中可用的语言。</span><span class="sxs-lookup"><span data-stu-id="a40b1-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="a40b1-107">**注意：** 若要检索支持自定义的语言，必须先在 Azure AD B2C 用户流上启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="a40b1-107">**Note:** To retrieve a language supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="a40b1-108">有关详细信息，请参阅[Update b2cIdentityUserFlow。](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="a40b1-108">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span> <span data-ttu-id="a40b1-109">默认情况下，在 Azure Active Directory 用户流 [中启用语言自定义](../resources/b2xidentityuserflow.md)。</span><span class="sxs-lookup"><span data-stu-id="a40b1-109">Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a40b1-110">权限</span><span class="sxs-lookup"><span data-stu-id="a40b1-110">Permissions</span></span>

<span data-ttu-id="a40b1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a40b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a40b1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a40b1-113">Permission type</span></span>      | <span data-ttu-id="a40b1-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a40b1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a40b1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a40b1-115">Delegated (work or school account)</span></span>|<span data-ttu-id="a40b1-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a40b1-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a40b1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a40b1-117">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a40b1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a40b1-118">Not supported.</span></span>|
|<span data-ttu-id="a40b1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a40b1-119">Application</span></span>|<span data-ttu-id="a40b1-120">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a40b1-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a40b1-121">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="a40b1-121">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a40b1-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a40b1-122">Global administrator</span></span>
* <span data-ttu-id="a40b1-123">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="a40b1-123">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a40b1-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a40b1-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a40b1-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="a40b1-125">Request headers</span></span>

|<span data-ttu-id="a40b1-126">名称</span><span class="sxs-lookup"><span data-stu-id="a40b1-126">Name</span></span>|<span data-ttu-id="a40b1-127">说明</span><span class="sxs-lookup"><span data-stu-id="a40b1-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a40b1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a40b1-128">Authorization</span></span>|<span data-ttu-id="a40b1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a40b1-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a40b1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a40b1-131">Request body</span></span>

<span data-ttu-id="a40b1-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a40b1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a40b1-133">响应</span><span class="sxs-lookup"><span data-stu-id="a40b1-133">Response</span></span>

<span data-ttu-id="a40b1-134">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a40b1-134">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a40b1-135">示例</span><span class="sxs-lookup"><span data-stu-id="a40b1-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a40b1-136">请求</span><span class="sxs-lookup"><span data-stu-id="a40b1-136">Request</span></span>

<span data-ttu-id="a40b1-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a40b1-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```

### <a name="response"></a><span data-ttu-id="a40b1-138">响应</span><span class="sxs-lookup"><span data-stu-id="a40b1-138">Response</span></span>

<span data-ttu-id="a40b1-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a40b1-139">The following is an example of the response.</span></span>

<span data-ttu-id="a40b1-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a40b1-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_Customer')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
