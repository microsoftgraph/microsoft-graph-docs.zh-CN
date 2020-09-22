---
title: 创建 publishedResource
description: 创建新的 **publishedResource** 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: be0c6eb175716509963b897f210044c5cde1ce2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027522"
---
# <a name="create-publishedresource"></a><span data-ttu-id="f3c6b-103">创建 publishedResource</span><span class="sxs-lookup"><span data-stu-id="f3c6b-103">Create publishedResource</span></span>

<span data-ttu-id="f3c6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3c6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3c6b-105">创建新的 [publishedResource](../resources/publishedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-105">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3c6b-106">权限</span><span class="sxs-lookup"><span data-stu-id="f3c6b-106">Permissions</span></span>

<span data-ttu-id="f3c6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3c6b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3c6b-109">Permission type</span></span>                        | <span data-ttu-id="f3c6b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3c6b-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3c6b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3c6b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3c6b-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3c6b-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="f3c6b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3c6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3c6b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-114">Not supported.</span></span> |
| <span data-ttu-id="f3c6b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3c6b-115">Application</span></span>                            | <span data-ttu-id="f3c6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3c6b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3c6b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="f3c6b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3c6b-118">Request headers</span></span>

| <span data-ttu-id="f3c6b-119">名称</span><span class="sxs-lookup"><span data-stu-id="f3c6b-119">Name</span></span>      |<span data-ttu-id="f3c6b-120">说明</span><span class="sxs-lookup"><span data-stu-id="f3c6b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3c6b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3c6b-121">Authorization</span></span> | <span data-ttu-id="f3c6b-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="f3c6b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3c6b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3c6b-123">Request body</span></span>

<span data-ttu-id="f3c6b-124">在请求正文中，提供 [publishedResource](../resources/publishedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-124">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="f3c6b-125">提供以下属性的值。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-125">Supply the values for the following properties.</span></span>

| <span data-ttu-id="f3c6b-126">属性</span><span class="sxs-lookup"><span data-stu-id="f3c6b-126">Property</span></span>     | <span data-ttu-id="f3c6b-127">类型</span><span class="sxs-lookup"><span data-stu-id="f3c6b-127">Type</span></span>        | <span data-ttu-id="f3c6b-128">说明</span><span class="sxs-lookup"><span data-stu-id="f3c6b-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f3c6b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f3c6b-129">displayName</span></span>|<span data-ttu-id="f3c6b-130">String</span><span class="sxs-lookup"><span data-stu-id="f3c6b-130">String</span></span>|<span data-ttu-id="f3c6b-131">PublishedResource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-131">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="f3c6b-132">resourceName</span><span class="sxs-lookup"><span data-stu-id="f3c6b-132">resourceName</span></span>|<span data-ttu-id="f3c6b-133">String</span><span class="sxs-lookup"><span data-stu-id="f3c6b-133">String</span></span>|<span data-ttu-id="f3c6b-134">PublishedResource 的名称。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-134">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="f3c6b-135">响应</span><span class="sxs-lookup"><span data-stu-id="f3c6b-135">Response</span></span>

<span data-ttu-id="f3c6b-136">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [publishedResource](../resources/publishedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-136">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3c6b-137">示例</span><span class="sxs-lookup"><span data-stu-id="f3c6b-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3c6b-138">请求</span><span class="sxs-lookup"><span data-stu-id="f3c6b-138">Request</span></span>

<span data-ttu-id="f3c6b-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3c6b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3c6b-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f3c6b-141">C#</span><span class="sxs-lookup"><span data-stu-id="f3c6b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3c6b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3c6b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3c6b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3c6b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f3c6b-144">响应</span><span class="sxs-lookup"><span data-stu-id="f3c6b-144">Response</span></span>

<span data-ttu-id="f3c6b-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-145">The following is an example of the response.</span></span>

> <span data-ttu-id="f3c6b-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f3c6b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


