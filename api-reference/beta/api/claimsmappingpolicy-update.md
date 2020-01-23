---
title: 更新 claimsmappingpolicy
description: 更新 claimsMappingPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6ffca9e41cdf51437ff421e472c5efa7c6faf671
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476326"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="b8d2f-103">更新 claimsmappingpolicy</span><span class="sxs-lookup"><span data-stu-id="b8d2f-103">Update claimsmappingpolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8d2f-104">更新[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-104">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8d2f-105">权限</span><span class="sxs-lookup"><span data-stu-id="b8d2f-105">Permissions</span></span>

<span data-ttu-id="b8d2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8d2f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8d2f-108">Permission type</span></span>                        | <span data-ttu-id="b8d2f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8d2f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8d2f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8d2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8d2f-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8d2f-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b8d2f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8d2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8d2f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-113">Not supported.</span></span> |
| <span data-ttu-id="b8d2f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8d2f-114">Application</span></span>                            | <span data-ttu-id="b8d2f-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8d2f-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8d2f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8d2f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b8d2f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8d2f-117">Request headers</span></span>

| <span data-ttu-id="b8d2f-118">名称</span><span class="sxs-lookup"><span data-stu-id="b8d2f-118">Name</span></span>       | <span data-ttu-id="b8d2f-119">说明</span><span class="sxs-lookup"><span data-stu-id="b8d2f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b8d2f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8d2f-120">Authorization</span></span> | <span data-ttu-id="b8d2f-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b8d2f-121">Bearer {token}</span></span> |
| <span data-ttu-id="b8d2f-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="b8d2f-122">Content-type</span></span> | <span data-ttu-id="b8d2f-123">application/json</span><span class="sxs-lookup"><span data-stu-id="b8d2f-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8d2f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8d2f-124">Request body</span></span>

<span data-ttu-id="b8d2f-125">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b8d2f-126">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8d2f-127">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b8d2f-128">属性</span><span class="sxs-lookup"><span data-stu-id="b8d2f-128">Property</span></span>     | <span data-ttu-id="b8d2f-129">类型</span><span class="sxs-lookup"><span data-stu-id="b8d2f-129">Type</span></span>        | <span data-ttu-id="b8d2f-130">说明</span><span class="sxs-lookup"><span data-stu-id="b8d2f-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8d2f-131">定义</span><span class="sxs-lookup"><span data-stu-id="b8d2f-131">definition</span></span>|<span data-ttu-id="b8d2f-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="b8d2f-132">String collection</span></span>| <span data-ttu-id="b8d2f-133">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-133">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="b8d2f-134">必需。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-134">Required.</span></span>|
|<span data-ttu-id="b8d2f-135">description</span><span class="sxs-lookup"><span data-stu-id="b8d2f-135">description</span></span>|<span data-ttu-id="b8d2f-136">String</span><span class="sxs-lookup"><span data-stu-id="b8d2f-136">String</span></span>| <span data-ttu-id="b8d2f-137">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-137">Description for this policy.</span></span>|
|<span data-ttu-id="b8d2f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b8d2f-138">displayName</span></span>|<span data-ttu-id="b8d2f-139">String</span><span class="sxs-lookup"><span data-stu-id="b8d2f-139">String</span></span>| <span data-ttu-id="b8d2f-140">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-140">Display name for this policy.</span></span> <span data-ttu-id="b8d2f-141">必填。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-141">Required.</span></span>|
|<span data-ttu-id="b8d2f-142">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b8d2f-142">isOrganizationDefault</span></span>|<span data-ttu-id="b8d2f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8d2f-143">Boolean</span></span>|<span data-ttu-id="b8d2f-144">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-144">If set to true, activates this policy.</span></span> <span data-ttu-id="b8d2f-145">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-145">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="b8d2f-146">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-146">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="b8d2f-147">响应</span><span class="sxs-lookup"><span data-stu-id="b8d2f-147">Response</span></span>

<span data-ttu-id="b8d2f-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8d2f-150">示例</span><span class="sxs-lookup"><span data-stu-id="b8d2f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8d2f-151">请求</span><span class="sxs-lookup"><span data-stu-id="b8d2f-151">Request</span></span>

<span data-ttu-id="b8d2f-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8d2f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8d2f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8d2f-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8d2f-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b8d2f-155">响应</span><span class="sxs-lookup"><span data-stu-id="b8d2f-155">Response</span></span>

<span data-ttu-id="b8d2f-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-156">The following is an example of the response.</span></span>

> <span data-ttu-id="b8d2f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b8d2f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
