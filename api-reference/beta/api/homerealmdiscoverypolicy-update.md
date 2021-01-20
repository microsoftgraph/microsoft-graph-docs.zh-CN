---
title: 更新 homerealmdiscoverypolicy
description: 更新 homeRealmDiscoveryPolicy 对象的属性。
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9e04d7ac91dedb7ef515741c86c29f3996d248f6
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910730"
---
# <a name="update-homerealmdiscoverypolicy"></a><span data-ttu-id="76deb-103">更新 homerealmdiscoverypolicy</span><span class="sxs-lookup"><span data-stu-id="76deb-103">Update homerealmdiscoverypolicy</span></span>

<span data-ttu-id="76deb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76deb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76deb-105">更新 [homeRealmDiscoveryPolicy 对象](../resources/homerealmdiscoverypolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="76deb-105">Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="76deb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="76deb-106">Permissions</span></span>

<span data-ttu-id="76deb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76deb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76deb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="76deb-109">Permission type</span></span>                        | <span data-ttu-id="76deb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76deb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76deb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76deb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="76deb-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="76deb-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="76deb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76deb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76deb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="76deb-114">Not supported.</span></span> |
| <span data-ttu-id="76deb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="76deb-115">Application</span></span>                            | <span data-ttu-id="76deb-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="76deb-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="76deb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76deb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76deb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="76deb-118">Request headers</span></span>

| <span data-ttu-id="76deb-119">名称</span><span class="sxs-lookup"><span data-stu-id="76deb-119">Name</span></span>       | <span data-ttu-id="76deb-120">说明</span><span class="sxs-lookup"><span data-stu-id="76deb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="76deb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="76deb-121">Authorization</span></span> | <span data-ttu-id="76deb-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="76deb-122">Bearer {token}</span></span> |
| <span data-ttu-id="76deb-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="76deb-123">Content-type</span></span> | <span data-ttu-id="76deb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76deb-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="76deb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="76deb-125">Request body</span></span>

<span data-ttu-id="76deb-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="76deb-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="76deb-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="76deb-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="76deb-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="76deb-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="76deb-129">属性</span><span class="sxs-lookup"><span data-stu-id="76deb-129">Property</span></span>     | <span data-ttu-id="76deb-130">类型</span><span class="sxs-lookup"><span data-stu-id="76deb-130">Type</span></span>        | <span data-ttu-id="76deb-131">说明</span><span class="sxs-lookup"><span data-stu-id="76deb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76deb-132">definition</span><span class="sxs-lookup"><span data-stu-id="76deb-132">definition</span></span>|<span data-ttu-id="76deb-133">String collection</span><span class="sxs-lookup"><span data-stu-id="76deb-133">String collection</span></span>| <span data-ttu-id="76deb-134">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="76deb-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="76deb-135">必需。</span><span class="sxs-lookup"><span data-stu-id="76deb-135">Required.</span></span>|
|<span data-ttu-id="76deb-136">description</span><span class="sxs-lookup"><span data-stu-id="76deb-136">description</span></span>|<span data-ttu-id="76deb-137">String</span><span class="sxs-lookup"><span data-stu-id="76deb-137">String</span></span>| <span data-ttu-id="76deb-138">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="76deb-138">Description for this policy.</span></span>|
|<span data-ttu-id="76deb-139">displayName</span><span class="sxs-lookup"><span data-stu-id="76deb-139">displayName</span></span>|<span data-ttu-id="76deb-140">String</span><span class="sxs-lookup"><span data-stu-id="76deb-140">String</span></span>| <span data-ttu-id="76deb-141">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="76deb-141">Display name for this policy.</span></span> <span data-ttu-id="76deb-142">必需。</span><span class="sxs-lookup"><span data-stu-id="76deb-142">Required.</span></span>|
|<span data-ttu-id="76deb-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="76deb-143">isOrganizationDefault</span></span>|<span data-ttu-id="76deb-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="76deb-144">Boolean</span></span>|<span data-ttu-id="76deb-145">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="76deb-145">If set to true, activates this policy.</span></span> <span data-ttu-id="76deb-146">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。</span><span class="sxs-lookup"><span data-stu-id="76deb-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="76deb-147">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="76deb-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="76deb-148">响应</span><span class="sxs-lookup"><span data-stu-id="76deb-148">Response</span></span>

<span data-ttu-id="76deb-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="76deb-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76deb-151">示例</span><span class="sxs-lookup"><span data-stu-id="76deb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="76deb-152">请求</span><span class="sxs-lookup"><span data-stu-id="76deb-152">Request</span></span>

<span data-ttu-id="76deb-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76deb-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76deb-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="76deb-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_homerealmdiscoverypolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="76deb-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76deb-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="76deb-156">C#</span><span class="sxs-lookup"><span data-stu-id="76deb-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76deb-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76deb-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76deb-158">Java</span><span class="sxs-lookup"><span data-stu-id="76deb-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76deb-159">响应</span><span class="sxs-lookup"><span data-stu-id="76deb-159">Response</span></span>

<span data-ttu-id="76deb-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76deb-160">The following is an example of the response.</span></span>

> <span data-ttu-id="76deb-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="76deb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


