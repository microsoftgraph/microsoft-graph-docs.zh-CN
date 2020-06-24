---
title: 更新 claimsmappingpolicy
description: 更新 claimsMappingPolicy 对象的属性。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f5434c73f7942a87babe21170bb2d82ca9f15c76
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846227"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="dcf54-103">更新 claimsmappingpolicy</span><span class="sxs-lookup"><span data-stu-id="dcf54-103">Update claimsmappingpolicy</span></span>

<span data-ttu-id="dcf54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcf54-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcf54-105">更新[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dcf54-105">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf54-106">权限</span><span class="sxs-lookup"><span data-stu-id="dcf54-106">Permissions</span></span>

<span data-ttu-id="dcf54-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dcf54-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dcf54-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf54-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcf54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcf54-109">Permission type</span></span>                        | <span data-ttu-id="dcf54-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcf54-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcf54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcf54-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcf54-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="dcf54-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="dcf54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcf54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf54-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcf54-114">Not supported.</span></span> |
| <span data-ttu-id="dcf54-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcf54-115">Application</span></span>                            | <span data-ttu-id="dcf54-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="dcf54-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf54-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcf54-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dcf54-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcf54-118">Request headers</span></span>

| <span data-ttu-id="dcf54-119">名称</span><span class="sxs-lookup"><span data-stu-id="dcf54-119">Name</span></span>       | <span data-ttu-id="dcf54-120">说明</span><span class="sxs-lookup"><span data-stu-id="dcf54-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dcf54-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf54-121">Authorization</span></span> | <span data-ttu-id="dcf54-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dcf54-122">Bearer {token}</span></span> |
| <span data-ttu-id="dcf54-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="dcf54-123">Content-type</span></span> | <span data-ttu-id="dcf54-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dcf54-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcf54-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcf54-125">Request body</span></span>

<span data-ttu-id="dcf54-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="dcf54-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dcf54-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="dcf54-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dcf54-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="dcf54-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dcf54-129">属性</span><span class="sxs-lookup"><span data-stu-id="dcf54-129">Property</span></span>     | <span data-ttu-id="dcf54-130">类型</span><span class="sxs-lookup"><span data-stu-id="dcf54-130">Type</span></span>        | <span data-ttu-id="dcf54-131">Description</span><span class="sxs-lookup"><span data-stu-id="dcf54-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dcf54-132">定义</span><span class="sxs-lookup"><span data-stu-id="dcf54-132">definition</span></span>|<span data-ttu-id="dcf54-133">String collection</span><span class="sxs-lookup"><span data-stu-id="dcf54-133">String collection</span></span>| <span data-ttu-id="dcf54-134">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="dcf54-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="dcf54-135">必需。</span><span class="sxs-lookup"><span data-stu-id="dcf54-135">Required.</span></span>|
|<span data-ttu-id="dcf54-136">description</span><span class="sxs-lookup"><span data-stu-id="dcf54-136">description</span></span>|<span data-ttu-id="dcf54-137">String</span><span class="sxs-lookup"><span data-stu-id="dcf54-137">String</span></span>| <span data-ttu-id="dcf54-138">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="dcf54-138">Description for this policy.</span></span>|
|<span data-ttu-id="dcf54-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dcf54-139">displayName</span></span>|<span data-ttu-id="dcf54-140">String</span><span class="sxs-lookup"><span data-stu-id="dcf54-140">String</span></span>| <span data-ttu-id="dcf54-141">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dcf54-141">Display name for this policy.</span></span> <span data-ttu-id="dcf54-142">必填。</span><span class="sxs-lookup"><span data-stu-id="dcf54-142">Required.</span></span>|
|<span data-ttu-id="dcf54-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="dcf54-143">isOrganizationDefault</span></span>|<span data-ttu-id="dcf54-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="dcf54-144">Boolean</span></span>|<span data-ttu-id="dcf54-145">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="dcf54-145">If set to true, activates this policy.</span></span> <span data-ttu-id="dcf54-146">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="dcf54-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="dcf54-147">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="dcf54-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="dcf54-148">响应</span><span class="sxs-lookup"><span data-stu-id="dcf54-148">Response</span></span>

<span data-ttu-id="dcf54-149">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="dcf54-149">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="dcf54-150">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="dcf54-150">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcf54-151">示例</span><span class="sxs-lookup"><span data-stu-id="dcf54-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcf54-152">请求</span><span class="sxs-lookup"><span data-stu-id="dcf54-152">Request</span></span>

<span data-ttu-id="dcf54-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dcf54-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcf54-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf54-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "type": "type-value"
}
```

### <a name="response"></a><span data-ttu-id="dcf54-155">响应</span><span class="sxs-lookup"><span data-stu-id="dcf54-155">Response</span></span>

<span data-ttu-id="dcf54-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dcf54-156">The following is an example of the response.</span></span>

> <span data-ttu-id="dcf54-157">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="dcf54-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dcf54-158">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="dcf54-158">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
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
  "description": "Update claimsmappingpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
