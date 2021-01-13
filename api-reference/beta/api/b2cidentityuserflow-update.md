---
title: 更新 b2cIdentityUserFlow
description: 更新 b2cIdentityUserFlow 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f579b4772a9ee496b6f702d418d6b577bd4915db
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843658"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="faf5f-103">更新 b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="faf5f-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="faf5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faf5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="faf5f-105">更新 [b2cIdentityUserFlow 对象](../resources/b2cidentityuserflow.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="faf5f-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="faf5f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="faf5f-106">Permissions</span></span>

<span data-ttu-id="faf5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="faf5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf5f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="faf5f-109">Permission type</span></span>      | <span data-ttu-id="faf5f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="faf5f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faf5f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="faf5f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="faf5f-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf5f-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="faf5f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="faf5f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="faf5f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="faf5f-114">Not supported.</span></span>|
|<span data-ttu-id="faf5f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="faf5f-115">Application</span></span>|<span data-ttu-id="faf5f-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf5f-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="faf5f-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="faf5f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="faf5f-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="faf5f-118">Global administrator</span></span>
* <span data-ttu-id="faf5f-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="faf5f-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="faf5f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="faf5f-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="faf5f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="faf5f-121">Request headers</span></span>

|<span data-ttu-id="faf5f-122">名称</span><span class="sxs-lookup"><span data-stu-id="faf5f-122">Name</span></span>|<span data-ttu-id="faf5f-123">说明</span><span class="sxs-lookup"><span data-stu-id="faf5f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="faf5f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="faf5f-124">Authorization</span></span>|<span data-ttu-id="faf5f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="faf5f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="faf5f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="faf5f-127">Content-Type</span></span>|<span data-ttu-id="faf5f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="faf5f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf5f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="faf5f-130">Request body</span></span>

<span data-ttu-id="faf5f-131">在请求正文中，提供 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faf5f-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="faf5f-132">下表显示创建 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)后可以更新的属性。</span><span class="sxs-lookup"><span data-stu-id="faf5f-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="faf5f-133">属性</span><span class="sxs-lookup"><span data-stu-id="faf5f-133">Property</span></span>|<span data-ttu-id="faf5f-134">类型</span><span class="sxs-lookup"><span data-stu-id="faf5f-134">Type</span></span>|<span data-ttu-id="faf5f-135">说明</span><span class="sxs-lookup"><span data-stu-id="faf5f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faf5f-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="faf5f-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="faf5f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf5f-137">Boolean</span></span>|<span data-ttu-id="faf5f-138">此属性决定语言自定义是否在 B2C 用户流中启用。</span><span class="sxs-lookup"><span data-stu-id="faf5f-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="faf5f-139">默认情况下，语言自定义不会在 B2C 用户流中启用。</span><span class="sxs-lookup"><span data-stu-id="faf5f-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="faf5f-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="faf5f-140">defaultLanguageTag</span></span>|<span data-ttu-id="faf5f-141">String</span><span class="sxs-lookup"><span data-stu-id="faf5f-141">String</span></span>|<span data-ttu-id="faf5f-142">指示在请求中没有指定 `ui_locale` 标签时使用的 b2cIdentityUserFlow 的默认语言。</span><span class="sxs-lookup"><span data-stu-id="faf5f-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="faf5f-143">此字段符合 [RFC 5646](https://tools.ietf.org/html/rfc5646)。</span><span class="sxs-lookup"><span data-stu-id="faf5f-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="faf5f-144">响应</span><span class="sxs-lookup"><span data-stu-id="faf5f-144">Response</span></span>

<span data-ttu-id="faf5f-145">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新 [的 b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="faf5f-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="faf5f-146">示例</span><span class="sxs-lookup"><span data-stu-id="faf5f-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="faf5f-147">请求</span><span class="sxs-lookup"><span data-stu-id="faf5f-147">Request</span></span>

<span data-ttu-id="faf5f-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="faf5f-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="faf5f-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="faf5f-149">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="faf5f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="faf5f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="faf5f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="faf5f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="faf5f-152">C#</span><span class="sxs-lookup"><span data-stu-id="faf5f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="faf5f-153">Java</span><span class="sxs-lookup"><span data-stu-id="faf5f-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="faf5f-154">响应</span><span class="sxs-lookup"><span data-stu-id="faf5f-154">Response</span></span>

<span data-ttu-id="faf5f-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="faf5f-155">The following is an example of the response.</span></span>

<span data-ttu-id="faf5f-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="faf5f-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
