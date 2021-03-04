---
title: 更新 b2cIdentityUserFlow
description: 更新 b2cIdentityUserFlow 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4ec3217af72d08d8dda103ec9304b25218344398
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438181"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="370f7-103">更新 b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="370f7-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="370f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="370f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="370f7-105">更新 [b2cIdentityUserFlow 对象](../resources/b2cidentityuserflow.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="370f7-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="370f7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="370f7-106">Permissions</span></span>

<span data-ttu-id="370f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="370f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="370f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="370f7-109">Permission type</span></span>      | <span data-ttu-id="370f7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="370f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="370f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="370f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="370f7-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="370f7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="370f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="370f7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="370f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="370f7-114">Not supported.</span></span>|
|<span data-ttu-id="370f7-115">Application</span><span class="sxs-lookup"><span data-stu-id="370f7-115">Application</span></span>|<span data-ttu-id="370f7-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="370f7-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="370f7-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="370f7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="370f7-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="370f7-118">Global administrator</span></span>
* <span data-ttu-id="370f7-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="370f7-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="370f7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="370f7-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="370f7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="370f7-121">Request headers</span></span>

|<span data-ttu-id="370f7-122">名称</span><span class="sxs-lookup"><span data-stu-id="370f7-122">Name</span></span>|<span data-ttu-id="370f7-123">说明</span><span class="sxs-lookup"><span data-stu-id="370f7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="370f7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="370f7-124">Authorization</span></span>|<span data-ttu-id="370f7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="370f7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="370f7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="370f7-127">Content-Type</span></span>|<span data-ttu-id="370f7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="370f7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="370f7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="370f7-130">Request body</span></span>

<span data-ttu-id="370f7-131">在请求正文中，提供 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="370f7-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="370f7-132">下表显示创建 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)后可以更新的属性。</span><span class="sxs-lookup"><span data-stu-id="370f7-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="370f7-133">属性</span><span class="sxs-lookup"><span data-stu-id="370f7-133">Property</span></span>|<span data-ttu-id="370f7-134">类型</span><span class="sxs-lookup"><span data-stu-id="370f7-134">Type</span></span>|<span data-ttu-id="370f7-135">说明</span><span class="sxs-lookup"><span data-stu-id="370f7-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="370f7-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="370f7-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="370f7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="370f7-137">Boolean</span></span>|<span data-ttu-id="370f7-138">此属性决定语言自定义是否在 B2C 用户流中启用。</span><span class="sxs-lookup"><span data-stu-id="370f7-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="370f7-139">默认情况下，语言自定义不会在 B2C 用户流中启用。</span><span class="sxs-lookup"><span data-stu-id="370f7-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="370f7-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="370f7-140">defaultLanguageTag</span></span>|<span data-ttu-id="370f7-141">String</span><span class="sxs-lookup"><span data-stu-id="370f7-141">String</span></span>|<span data-ttu-id="370f7-142">指示在请求中没有指定 `ui_locale` 标签时使用的 b2cIdentityUserFlow 的默认语言。</span><span class="sxs-lookup"><span data-stu-id="370f7-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="370f7-143">此字段符合 [RFC 5646](https://tools.ietf.org/html/rfc5646)。</span><span class="sxs-lookup"><span data-stu-id="370f7-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="370f7-144">响应</span><span class="sxs-lookup"><span data-stu-id="370f7-144">Response</span></span>

<span data-ttu-id="370f7-145">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` [的 b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="370f7-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="370f7-146">示例</span><span class="sxs-lookup"><span data-stu-id="370f7-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="370f7-147">请求</span><span class="sxs-lookup"><span data-stu-id="370f7-147">Request</span></span>

<span data-ttu-id="370f7-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="370f7-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="370f7-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="370f7-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cidentityuserflow"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp
Content-Type: application/json
Content-length: 469

{
  "isLanguageCustomizationEnabled": true,
  "defaultLanguageTag": "en",
}
```
# <a name="javascript"></a>[<span data-ttu-id="370f7-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="370f7-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="370f7-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="370f7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="370f7-152">C#</span><span class="sxs-lookup"><span data-stu-id="370f7-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="370f7-153">Java</span><span class="sxs-lookup"><span data-stu-id="370f7-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="370f7-154">响应</span><span class="sxs-lookup"><span data-stu-id="370f7-154">Response</span></span>

<span data-ttu-id="370f7-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="370f7-155">The following is an example of the response.</span></span>

<span data-ttu-id="370f7-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="370f7-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
}
-->

``` http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
