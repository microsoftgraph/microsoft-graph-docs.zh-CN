---
title: 更新 activitybasedtimeoutpolicy
description: 更新 activityBasedTimeoutPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7a3c2d47e2de2fedf69d502dd920998f6a32996e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441779"
---
# <a name="update-activitybasedtimeoutpolicy"></a><span data-ttu-id="ff702-103">更新 activitybasedtimeoutpolicy</span><span class="sxs-lookup"><span data-stu-id="ff702-103">Update activitybasedtimeoutpolicy</span></span>

<span data-ttu-id="ff702-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ff702-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff702-105">更新[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff702-105">Update the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff702-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff702-106">Permissions</span></span>

<span data-ttu-id="ff702-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff702-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff702-109">Permission type</span></span>                        | <span data-ttu-id="ff702-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff702-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff702-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff702-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff702-112">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff702-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ff702-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff702-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff702-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff702-114">Not supported.</span></span> |
| <span data-ttu-id="ff702-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff702-115">Application</span></span>                            | <span data-ttu-id="ff702-116">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff702-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff702-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff702-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ff702-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff702-118">Request headers</span></span>

| <span data-ttu-id="ff702-119">名称</span><span class="sxs-lookup"><span data-stu-id="ff702-119">Name</span></span>       | <span data-ttu-id="ff702-120">说明</span><span class="sxs-lookup"><span data-stu-id="ff702-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ff702-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff702-121">Authorization</span></span> | <span data-ttu-id="ff702-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ff702-122">Bearer {token}</span></span> |
| <span data-ttu-id="ff702-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="ff702-123">Content-type</span></span> | <span data-ttu-id="ff702-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff702-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff702-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff702-125">Request body</span></span>

<span data-ttu-id="ff702-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ff702-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ff702-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ff702-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ff702-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ff702-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff702-129">属性</span><span class="sxs-lookup"><span data-stu-id="ff702-129">Property</span></span>     | <span data-ttu-id="ff702-130">类型</span><span class="sxs-lookup"><span data-stu-id="ff702-130">Type</span></span>        | <span data-ttu-id="ff702-131">说明</span><span class="sxs-lookup"><span data-stu-id="ff702-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff702-132">定义</span><span class="sxs-lookup"><span data-stu-id="ff702-132">definition</span></span>|<span data-ttu-id="ff702-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="ff702-133">String collection</span></span>| <span data-ttu-id="ff702-134">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="ff702-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="ff702-135">必需。</span><span class="sxs-lookup"><span data-stu-id="ff702-135">Required.</span></span>|
|<span data-ttu-id="ff702-136">description</span><span class="sxs-lookup"><span data-stu-id="ff702-136">description</span></span>|<span data-ttu-id="ff702-137">String</span><span class="sxs-lookup"><span data-stu-id="ff702-137">String</span></span>| <span data-ttu-id="ff702-138">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ff702-138">Description for this policy.</span></span>|
|<span data-ttu-id="ff702-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ff702-139">displayName</span></span>|<span data-ttu-id="ff702-140">String</span><span class="sxs-lookup"><span data-stu-id="ff702-140">String</span></span>| <span data-ttu-id="ff702-141">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ff702-141">Display name for this policy.</span></span> <span data-ttu-id="ff702-142">必填。</span><span class="sxs-lookup"><span data-stu-id="ff702-142">Required.</span></span>|
|<span data-ttu-id="ff702-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="ff702-143">isOrganizationDefault</span></span>|<span data-ttu-id="ff702-144">布尔</span><span class="sxs-lookup"><span data-stu-id="ff702-144">Boolean</span></span>|<span data-ttu-id="ff702-145">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="ff702-145">If set to true, activates this policy.</span></span> <span data-ttu-id="ff702-146">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="ff702-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ff702-147">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="ff702-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ff702-148">响应</span><span class="sxs-lookup"><span data-stu-id="ff702-148">Response</span></span>

<span data-ttu-id="ff702-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ff702-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff702-151">示例</span><span class="sxs-lookup"><span data-stu-id="ff702-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff702-152">请求</span><span class="sxs-lookup"><span data-stu-id="ff702-152">Request</span></span>

<span data-ttu-id="ff702-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff702-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff702-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff702-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_activitybasedtimeoutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
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
# <a name="javascript"></a>[<span data-ttu-id="ff702-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff702-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff702-156">响应</span><span class="sxs-lookup"><span data-stu-id="ff702-156">Response</span></span>

<span data-ttu-id="ff702-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff702-157">The following is an example of the response.</span></span>

> <span data-ttu-id="ff702-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ff702-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
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
  "description": "Update activitybasedtimeoutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
