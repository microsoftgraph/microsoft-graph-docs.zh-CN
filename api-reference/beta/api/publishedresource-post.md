---
title: 创建 publishedResource
description: 创建新的**publishedResource**对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbb9bd814d8bb7947628145c62eb7717a4f2f83c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412339"
---
# <a name="create-publishedresource"></a><span data-ttu-id="2d13f-103">创建 publishedResource</span><span class="sxs-lookup"><span data-stu-id="2d13f-103">Create publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d13f-104">创建新的[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d13f-104">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d13f-105">权限</span><span class="sxs-lookup"><span data-stu-id="2d13f-105">Permissions</span></span>

<span data-ttu-id="2d13f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d13f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d13f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d13f-108">Permission type</span></span>                        | <span data-ttu-id="2d13f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d13f-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d13f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d13f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d13f-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="2d13f-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="2d13f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d13f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d13f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d13f-113">Not supported.</span></span> |
| <span data-ttu-id="2d13f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d13f-114">Application</span></span>                            | <span data-ttu-id="2d13f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d13f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d13f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d13f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="2d13f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d13f-117">Request headers</span></span>

| <span data-ttu-id="2d13f-118">名称</span><span class="sxs-lookup"><span data-stu-id="2d13f-118">Name</span></span>      |<span data-ttu-id="2d13f-119">说明</span><span class="sxs-lookup"><span data-stu-id="2d13f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d13f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d13f-120">Authorization</span></span> | <span data-ttu-id="2d13f-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="2d13f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d13f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d13f-122">Request body</span></span>

<span data-ttu-id="2d13f-123">在请求正文中, 提供[publishedResource](../resources/publishedresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d13f-123">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="2d13f-124">提供以下属性的值。</span><span class="sxs-lookup"><span data-stu-id="2d13f-124">Supply the values for the following properties.</span></span>

| <span data-ttu-id="2d13f-125">属性</span><span class="sxs-lookup"><span data-stu-id="2d13f-125">Property</span></span>     | <span data-ttu-id="2d13f-126">类型</span><span class="sxs-lookup"><span data-stu-id="2d13f-126">Type</span></span>        | <span data-ttu-id="2d13f-127">说明</span><span class="sxs-lookup"><span data-stu-id="2d13f-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d13f-128">displayName</span><span class="sxs-lookup"><span data-stu-id="2d13f-128">displayName</span></span>|<span data-ttu-id="2d13f-129">String</span><span class="sxs-lookup"><span data-stu-id="2d13f-129">String</span></span>|<span data-ttu-id="2d13f-130">PublishedResource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2d13f-130">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="2d13f-131">resourceName</span><span class="sxs-lookup"><span data-stu-id="2d13f-131">resourceName</span></span>|<span data-ttu-id="2d13f-132">String</span><span class="sxs-lookup"><span data-stu-id="2d13f-132">String</span></span>|<span data-ttu-id="2d13f-133">PublishedResource 的名称。</span><span class="sxs-lookup"><span data-stu-id="2d13f-133">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="2d13f-134">响应</span><span class="sxs-lookup"><span data-stu-id="2d13f-134">Response</span></span>

<span data-ttu-id="2d13f-135">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d13f-135">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d13f-136">示例</span><span class="sxs-lookup"><span data-stu-id="2d13f-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d13f-137">请求</span><span class="sxs-lookup"><span data-stu-id="2d13f-137">Request</span></span>

<span data-ttu-id="2d13f-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2d13f-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2d13f-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2d13f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_publishedresource_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources
Content-Type: application/json

{
    "displayName": "New provisioning",
    "resourceName": "domain1.contoso.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d13f-140">C#</span><span class="sxs-lookup"><span data-stu-id="2d13f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d13f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d13f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d13f-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="2d13f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d13f-143">响应</span><span class="sxs-lookup"><span data-stu-id="2d13f-143">Response</span></span>

<span data-ttu-id="2d13f-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2d13f-144">The following is an example of the response.</span></span>

> <span data-ttu-id="2d13f-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2d13f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 201 Created

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "publishingType": "provisioning",
    "displayName": "New provisionin",
    "resourceName": "domain1.contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
