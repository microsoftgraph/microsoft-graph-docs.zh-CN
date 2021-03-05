---
title: 更新 tokenIssuancePolicy
description: 更新 tokenIssuancePolicy 对象的属性。
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6779f7db60278cbd6df4c08007af5c0d527e80a8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448903"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="8cf6f-103">更新 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="8cf6f-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="8cf6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cf6f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8cf6f-105">更新 [tokenIssuancePolicy 对象](../resources/tokenIssuancePolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cf6f-106">权限</span><span class="sxs-lookup"><span data-stu-id="8cf6f-106">Permissions</span></span>

<span data-ttu-id="8cf6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cf6f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cf6f-109">Permission type</span></span>                        | <span data-ttu-id="8cf6f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cf6f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8cf6f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cf6f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cf6f-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8cf6f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8cf6f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cf6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cf6f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-114">Not supported.</span></span> |
| <span data-ttu-id="8cf6f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cf6f-115">Application</span></span>                            | <span data-ttu-id="8cf6f-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8cf6f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cf6f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cf6f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8cf6f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cf6f-118">Request headers</span></span>

| <span data-ttu-id="8cf6f-119">名称</span><span class="sxs-lookup"><span data-stu-id="8cf6f-119">Name</span></span>       | <span data-ttu-id="8cf6f-120">说明</span><span class="sxs-lookup"><span data-stu-id="8cf6f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8cf6f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cf6f-121">Authorization</span></span> | <span data-ttu-id="8cf6f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cf6f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="8cf6f-124">Content-type</span></span> | <span data-ttu-id="8cf6f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8cf6f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cf6f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cf6f-127">Request body</span></span>

<span data-ttu-id="8cf6f-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8cf6f-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8cf6f-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8cf6f-131">属性</span><span class="sxs-lookup"><span data-stu-id="8cf6f-131">Property</span></span>     | <span data-ttu-id="8cf6f-132">类型</span><span class="sxs-lookup"><span data-stu-id="8cf6f-132">Type</span></span>        | <span data-ttu-id="8cf6f-133">说明</span><span class="sxs-lookup"><span data-stu-id="8cf6f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cf6f-134">definition</span><span class="sxs-lookup"><span data-stu-id="8cf6f-134">definition</span></span>|<span data-ttu-id="8cf6f-135">String collection</span><span class="sxs-lookup"><span data-stu-id="8cf6f-135">String collection</span></span>| <span data-ttu-id="8cf6f-136">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="8cf6f-137">必需。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-137">Required.</span></span>|
|<span data-ttu-id="8cf6f-138">description</span><span class="sxs-lookup"><span data-stu-id="8cf6f-138">description</span></span>|<span data-ttu-id="8cf6f-139">String</span><span class="sxs-lookup"><span data-stu-id="8cf6f-139">String</span></span>| <span data-ttu-id="8cf6f-140">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-140">Description for this policy.</span></span>|
|<span data-ttu-id="8cf6f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8cf6f-141">displayName</span></span>|<span data-ttu-id="8cf6f-142">String</span><span class="sxs-lookup"><span data-stu-id="8cf6f-142">String</span></span>| <span data-ttu-id="8cf6f-143">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-143">Display name for this policy.</span></span> <span data-ttu-id="8cf6f-144">必填。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-144">Required.</span></span>|
|<span data-ttu-id="8cf6f-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="8cf6f-145">isOrganizationDefault</span></span>|<span data-ttu-id="8cf6f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cf6f-146">Boolean</span></span>|<span data-ttu-id="8cf6f-147">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-147">If set to true, activates this policy.</span></span> <span data-ttu-id="8cf6f-148">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认设置。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="8cf6f-149">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="8cf6f-150">响应</span><span class="sxs-lookup"><span data-stu-id="8cf6f-150">Response</span></span>

<span data-ttu-id="8cf6f-p108">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cf6f-153">示例</span><span class="sxs-lookup"><span data-stu-id="8cf6f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cf6f-154">请求</span><span class="sxs-lookup"><span data-stu-id="8cf6f-154">Request</span></span>

<span data-ttu-id="8cf6f-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8cf6f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cf6f-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tokenissuancepolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="8cf6f-157">C#</span><span class="sxs-lookup"><span data-stu-id="8cf6f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cf6f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cf6f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cf6f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cf6f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cf6f-160">Java</span><span class="sxs-lookup"><span data-stu-id="8cf6f-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tokenissuancepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8cf6f-161">响应</span><span class="sxs-lookup"><span data-stu-id="8cf6f-161">Response</span></span>

<span data-ttu-id="8cf6f-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-162">The following is an example of the response.</span></span>

> <span data-ttu-id="8cf6f-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8cf6f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Update tokenissuancepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

