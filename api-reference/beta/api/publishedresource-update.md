---
title: 更新 publishedResource
description: 更新 [publishedResource 对象](../resources/publishedresource.md) 的属性。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 22544845ededf639bc71f14dec72a7163ded7c90
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055153"
---
# <a name="update-publishedresource"></a><span data-ttu-id="1a3ec-103">更新 publishedResource</span><span class="sxs-lookup"><span data-stu-id="1a3ec-103">Update publishedResource</span></span>

<span data-ttu-id="1a3ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a3ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a3ec-105">更新 publishedresource  [publishedResource 对象](../resources/publishedresource.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-105">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a3ec-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a3ec-106">Permissions</span></span>

<span data-ttu-id="1a3ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a3ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a3ec-109">Permission type</span></span>                        | <span data-ttu-id="1a3ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a3ec-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="1a3ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a3ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a3ec-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a3ec-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="1a3ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a3ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a3ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-114">Not supported.</span></span> |
| <span data-ttu-id="1a3ec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a3ec-115">Application</span></span>                            | <span data-ttu-id="1a3ec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a3ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a3ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="1a3ec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a3ec-118">Request headers</span></span>

| <span data-ttu-id="1a3ec-119">名称</span><span class="sxs-lookup"><span data-stu-id="1a3ec-119">Name</span></span>       | <span data-ttu-id="1a3ec-120">说明</span><span class="sxs-lookup"><span data-stu-id="1a3ec-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1a3ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a3ec-121">Authorization</span></span> | <span data-ttu-id="1a3ec-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1a3ec-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a3ec-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a3ec-123">Request body</span></span>

<span data-ttu-id="1a3ec-124">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="1a3ec-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1a3ec-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="1a3ec-127">下表列出了可更新的属性。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-127">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="1a3ec-128">属性</span><span class="sxs-lookup"><span data-stu-id="1a3ec-128">Property</span></span>     | <span data-ttu-id="1a3ec-129">类型</span><span class="sxs-lookup"><span data-stu-id="1a3ec-129">Type</span></span>        | <span data-ttu-id="1a3ec-130">说明</span><span class="sxs-lookup"><span data-stu-id="1a3ec-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a3ec-131">displayName</span><span class="sxs-lookup"><span data-stu-id="1a3ec-131">displayName</span></span>|<span data-ttu-id="1a3ec-132">String</span><span class="sxs-lookup"><span data-stu-id="1a3ec-132">String</span></span>|<span data-ttu-id="1a3ec-133">表示本地已发布资源名称。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-133">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="1a3ec-134">响应</span><span class="sxs-lookup"><span data-stu-id="1a3ec-134">Response</span></span>

<span data-ttu-id="1a3ec-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1a3ec-136">示例</span><span class="sxs-lookup"><span data-stu-id="1a3ec-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a3ec-137">请求</span><span class="sxs-lookup"><span data-stu-id="1a3ec-137">Request</span></span>

<span data-ttu-id="1a3ec-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a3ec-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a3ec-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_publishedresource"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d

{
    "displayName": "Demo provisioning (updated)"
}
```
# <a name="c"></a>[<span data-ttu-id="1a3ec-140">C#</span><span class="sxs-lookup"><span data-stu-id="1a3ec-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a3ec-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a3ec-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a3ec-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a3ec-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a3ec-143">Java</span><span class="sxs-lookup"><span data-stu-id="1a3ec-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a3ec-144">响应</span><span class="sxs-lookup"><span data-stu-id="1a3ec-144">Response</span></span>

<span data-ttu-id="1a3ec-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-145">The following is an example of the response.</span></span>

> <span data-ttu-id="1a3ec-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1a3ec-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update publishedresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



