---
title: 更新 homerealmdiscoverypolicy
description: 更新 homeRealmDiscoveryPolicy 对象的属性。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7c46a8c7e46a9289bc47666b70dbf1d364d9467f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048685"
---
# <a name="update-homerealmdiscoverypolicy"></a><span data-ttu-id="ae4d7-103">更新 homerealmdiscoverypolicy</span><span class="sxs-lookup"><span data-stu-id="ae4d7-103">Update homerealmdiscoverypolicy</span></span>

<span data-ttu-id="ae4d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae4d7-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ae4d7-105">更新 [homeRealmDiscoveryPolicy 对象](../resources/homerealmdiscoverypolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-105">Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae4d7-106">权限</span><span class="sxs-lookup"><span data-stu-id="ae4d7-106">Permissions</span></span>

<span data-ttu-id="ae4d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae4d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae4d7-109">Permission type</span></span>                        | <span data-ttu-id="ae4d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae4d7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ae4d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae4d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae4d7-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae4d7-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ae4d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae4d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae4d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-114">Not supported.</span></span> |
| <span data-ttu-id="ae4d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae4d7-115">Application</span></span>                            | <span data-ttu-id="ae4d7-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae4d7-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae4d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae4d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ae4d7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae4d7-118">Request headers</span></span>

| <span data-ttu-id="ae4d7-119">名称</span><span class="sxs-lookup"><span data-stu-id="ae4d7-119">Name</span></span>       | <span data-ttu-id="ae4d7-120">说明</span><span class="sxs-lookup"><span data-stu-id="ae4d7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ae4d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae4d7-121">Authorization</span></span> | <span data-ttu-id="ae4d7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae4d7-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ae4d7-124">Content-type</span></span> | <span data-ttu-id="ae4d7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ae4d7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae4d7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae4d7-127">Request body</span></span>

<span data-ttu-id="ae4d7-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ae4d7-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ae4d7-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ae4d7-131">属性</span><span class="sxs-lookup"><span data-stu-id="ae4d7-131">Property</span></span>     | <span data-ttu-id="ae4d7-132">类型</span><span class="sxs-lookup"><span data-stu-id="ae4d7-132">Type</span></span>        | <span data-ttu-id="ae4d7-133">说明</span><span class="sxs-lookup"><span data-stu-id="ae4d7-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ae4d7-134">definition</span><span class="sxs-lookup"><span data-stu-id="ae4d7-134">definition</span></span>|<span data-ttu-id="ae4d7-135">字符串集合</span><span class="sxs-lookup"><span data-stu-id="ae4d7-135">String collection</span></span>| <span data-ttu-id="ae4d7-136">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="ae4d7-137">必需。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-137">Required.</span></span>|
|<span data-ttu-id="ae4d7-138">description</span><span class="sxs-lookup"><span data-stu-id="ae4d7-138">description</span></span>|<span data-ttu-id="ae4d7-139">String</span><span class="sxs-lookup"><span data-stu-id="ae4d7-139">String</span></span>| <span data-ttu-id="ae4d7-140">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-140">Description for this policy.</span></span>|
|<span data-ttu-id="ae4d7-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ae4d7-141">displayName</span></span>|<span data-ttu-id="ae4d7-142">String</span><span class="sxs-lookup"><span data-stu-id="ae4d7-142">String</span></span>| <span data-ttu-id="ae4d7-143">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-143">Display name for this policy.</span></span> <span data-ttu-id="ae4d7-144">必需。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-144">Required.</span></span>|
|<span data-ttu-id="ae4d7-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="ae4d7-145">isOrganizationDefault</span></span>|<span data-ttu-id="ae4d7-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="ae4d7-146">Boolean</span></span>|<span data-ttu-id="ae4d7-147">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-147">If set to true, activates this policy.</span></span> <span data-ttu-id="ae4d7-148">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ae4d7-149">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ae4d7-150">响应</span><span class="sxs-lookup"><span data-stu-id="ae4d7-150">Response</span></span>

<span data-ttu-id="ae4d7-p108">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae4d7-153">示例</span><span class="sxs-lookup"><span data-stu-id="ae4d7-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae4d7-154">请求</span><span class="sxs-lookup"><span data-stu-id="ae4d7-154">Request</span></span>

<span data-ttu-id="ae4d7-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae4d7-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae4d7-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_homerealmdiscoverypolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="ae4d7-157">C#</span><span class="sxs-lookup"><span data-stu-id="ae4d7-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae4d7-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae4d7-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae4d7-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae4d7-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae4d7-160">Java</span><span class="sxs-lookup"><span data-stu-id="ae4d7-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ae4d7-161">响应</span><span class="sxs-lookup"><span data-stu-id="ae4d7-161">Response</span></span>

<span data-ttu-id="ae4d7-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-162">The following is an example of the response.</span></span>

> <span data-ttu-id="ae4d7-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ae4d7-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update homerealmdiscoverypolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

