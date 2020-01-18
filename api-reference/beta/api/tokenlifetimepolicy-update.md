---
title: 更新 tokenlifetimepolicy
description: 更新 tokenLifetimePolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3963da371b775baa5ec7b8b3177bd40f9d9cebcb
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234191"
---
# <a name="update-tokenlifetimepolicy"></a><span data-ttu-id="0ca56-103">更新 tokenlifetimepolicy</span><span class="sxs-lookup"><span data-stu-id="0ca56-103">Update tokenlifetimepolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ca56-104">更新[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ca56-104">Update the properties of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ca56-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="0ca56-105">Permissions</span></span>

<span data-ttu-id="0ca56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ca56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ca56-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ca56-108">Permission type</span></span>                        | <span data-ttu-id="0ca56-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ca56-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ca56-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ca56-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ca56-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ca56-111">Policy.ReadWrite.ApplicationConfiguration</span></span>|
| <span data-ttu-id="0ca56-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ca56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ca56-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ca56-113">Not supported.</span></span> |
| <span data-ttu-id="0ca56-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ca56-114">Application</span></span>                            | <span data-ttu-id="0ca56-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ca56-115">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ca56-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ca56-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ca56-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ca56-117">Request headers</span></span>

| <span data-ttu-id="0ca56-118">名称</span><span class="sxs-lookup"><span data-stu-id="0ca56-118">Name</span></span>       | <span data-ttu-id="0ca56-119">说明</span><span class="sxs-lookup"><span data-stu-id="0ca56-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0ca56-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ca56-120">Authorization</span></span> | <span data-ttu-id="0ca56-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0ca56-121">Bearer {token}</span></span> |
| <span data-ttu-id="0ca56-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="0ca56-122">Content-type</span></span> | <span data-ttu-id="0ca56-123">application/json</span><span class="sxs-lookup"><span data-stu-id="0ca56-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ca56-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ca56-124">Request body</span></span>

<span data-ttu-id="0ca56-125">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0ca56-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0ca56-126">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0ca56-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0ca56-127">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0ca56-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ca56-128">属性</span><span class="sxs-lookup"><span data-stu-id="0ca56-128">Property</span></span>     | <span data-ttu-id="0ca56-129">类型</span><span class="sxs-lookup"><span data-stu-id="0ca56-129">Type</span></span>        | <span data-ttu-id="0ca56-130">说明</span><span class="sxs-lookup"><span data-stu-id="0ca56-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ca56-131">定义</span><span class="sxs-lookup"><span data-stu-id="0ca56-131">definition</span></span>|<span data-ttu-id="0ca56-132">String collection</span><span class="sxs-lookup"><span data-stu-id="0ca56-132">String collection</span></span>| <span data-ttu-id="0ca56-133">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="0ca56-133">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="0ca56-134">必需。</span><span class="sxs-lookup"><span data-stu-id="0ca56-134">Required.</span></span>|
|<span data-ttu-id="0ca56-135">description</span><span class="sxs-lookup"><span data-stu-id="0ca56-135">description</span></span>|<span data-ttu-id="0ca56-136">String</span><span class="sxs-lookup"><span data-stu-id="0ca56-136">String</span></span>| <span data-ttu-id="0ca56-137">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="0ca56-137">Description for this policy.</span></span>|
|<span data-ttu-id="0ca56-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0ca56-138">displayName</span></span>|<span data-ttu-id="0ca56-139">String</span><span class="sxs-lookup"><span data-stu-id="0ca56-139">String</span></span>| <span data-ttu-id="0ca56-140">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0ca56-140">Display name for this policy.</span></span> <span data-ttu-id="0ca56-141">必需。</span><span class="sxs-lookup"><span data-stu-id="0ca56-141">Required.</span></span>|
|<span data-ttu-id="0ca56-142">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="0ca56-142">isOrganizationDefault</span></span>|<span data-ttu-id="0ca56-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca56-143">Boolean</span></span>|<span data-ttu-id="0ca56-144">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="0ca56-144">If set to true, activates this policy.</span></span> <span data-ttu-id="0ca56-145">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="0ca56-145">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="0ca56-146">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="0ca56-146">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="0ca56-147">响应</span><span class="sxs-lookup"><span data-stu-id="0ca56-147">Response</span></span>

<span data-ttu-id="0ca56-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0ca56-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ca56-150">示例</span><span class="sxs-lookup"><span data-stu-id="0ca56-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ca56-151">请求</span><span class="sxs-lookup"><span data-stu-id="0ca56-151">Request</span></span>

<span data-ttu-id="0ca56-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ca56-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tokenlifetimepolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
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

### <a name="response"></a><span data-ttu-id="0ca56-153">响应</span><span class="sxs-lookup"><span data-stu-id="0ca56-153">Response</span></span>

<span data-ttu-id="0ca56-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ca56-154">The following is an example of the response.</span></span>

> <span data-ttu-id="0ca56-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0ca56-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Update tokenlifetimepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->