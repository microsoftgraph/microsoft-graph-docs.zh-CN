---
title: 获取 userFlowLanguageConfiguration
description: 读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 25fa30b9904854ce027c503cf738cabd55ce5567
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955250"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="44518-103">获取 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="44518-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="44518-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44518-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44518-105">读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44518-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="44518-106">这些对象表示用户流中可用的语言。</span><span class="sxs-lookup"><span data-stu-id="44518-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="44518-107">**注意：** 若要检索受自定义支持的语言，必须先对 Azure AD B2C 用户流启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="44518-107">**Note:** To retrieve a language supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="44518-108">有关详细信息，请参阅更新 [b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md)。</span><span class="sxs-lookup"><span data-stu-id="44518-108">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span> <span data-ttu-id="44518-109">默认情况下，在 Azure Active Directory 用户流 [中启用语言自定义](../resources/b2xidentityuserflow.md)。</span><span class="sxs-lookup"><span data-stu-id="44518-109">Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="44518-110">权限</span><span class="sxs-lookup"><span data-stu-id="44518-110">Permissions</span></span>

<span data-ttu-id="44518-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44518-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44518-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="44518-113">Permission type</span></span>      | <span data-ttu-id="44518-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44518-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44518-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44518-115">Delegated (work or school account)</span></span>|<span data-ttu-id="44518-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44518-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="44518-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44518-117">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="44518-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="44518-118">Not supported.</span></span>|
|<span data-ttu-id="44518-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="44518-119">Application</span></span>|<span data-ttu-id="44518-120">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44518-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="44518-121">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="44518-121">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="44518-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="44518-122">Global administrator</span></span>
* <span data-ttu-id="44518-123">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="44518-123">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="44518-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44518-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="44518-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="44518-125">Request headers</span></span>

|<span data-ttu-id="44518-126">名称</span><span class="sxs-lookup"><span data-stu-id="44518-126">Name</span></span>|<span data-ttu-id="44518-127">说明</span><span class="sxs-lookup"><span data-stu-id="44518-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="44518-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="44518-128">Authorization</span></span>|<span data-ttu-id="44518-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44518-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44518-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="44518-131">Request body</span></span>

<span data-ttu-id="44518-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44518-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44518-133">响应</span><span class="sxs-lookup"><span data-stu-id="44518-133">Response</span></span>

<span data-ttu-id="44518-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44518-134">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44518-135">示例</span><span class="sxs-lookup"><span data-stu-id="44518-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44518-136">请求</span><span class="sxs-lookup"><span data-stu-id="44518-136">Request</span></span>

<span data-ttu-id="44518-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="44518-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="44518-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="44518-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```
# <a name="c"></a>[<span data-ttu-id="44518-139">C#</span><span class="sxs-lookup"><span data-stu-id="44518-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44518-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44518-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44518-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44518-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44518-142">Java</span><span class="sxs-lookup"><span data-stu-id="44518-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="44518-143">响应</span><span class="sxs-lookup"><span data-stu-id="44518-143">Response</span></span>

<span data-ttu-id="44518-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="44518-144">The following is an example of the response.</span></span>

<span data-ttu-id="44518-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44518-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
