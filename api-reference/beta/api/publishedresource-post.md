---
title: 创建 publishedResource
description: 创建新的 **publishedResource** 对象。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0cf0b586010b6d68a36f4d710bc24f0035ecafa7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055160"
---
# <a name="create-publishedresource"></a><span data-ttu-id="3fa58-103">创建 publishedResource</span><span class="sxs-lookup"><span data-stu-id="3fa58-103">Create publishedResource</span></span>

<span data-ttu-id="3fa58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fa58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fa58-105">创建新的 [publishedResource](../resources/publishedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3fa58-105">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fa58-106">权限</span><span class="sxs-lookup"><span data-stu-id="3fa58-106">Permissions</span></span>

<span data-ttu-id="3fa58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3fa58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fa58-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fa58-109">Permission type</span></span>                        | <span data-ttu-id="3fa58-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3fa58-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fa58-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fa58-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3fa58-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa58-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="3fa58-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fa58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fa58-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fa58-114">Not supported.</span></span> |
| <span data-ttu-id="3fa58-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fa58-115">Application</span></span>                            | <span data-ttu-id="3fa58-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fa58-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fa58-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fa58-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="3fa58-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fa58-118">Request headers</span></span>

| <span data-ttu-id="3fa58-119">名称</span><span class="sxs-lookup"><span data-stu-id="3fa58-119">Name</span></span>      |<span data-ttu-id="3fa58-120">说明</span><span class="sxs-lookup"><span data-stu-id="3fa58-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3fa58-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa58-121">Authorization</span></span> | <span data-ttu-id="3fa58-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="3fa58-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fa58-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fa58-123">Request body</span></span>

<span data-ttu-id="3fa58-124">在请求正文中，提供 [publishedResource](../resources/publishedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fa58-124">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="3fa58-125">提供以下属性的值。</span><span class="sxs-lookup"><span data-stu-id="3fa58-125">Supply the values for the following properties.</span></span>

| <span data-ttu-id="3fa58-126">属性</span><span class="sxs-lookup"><span data-stu-id="3fa58-126">Property</span></span>     | <span data-ttu-id="3fa58-127">类型</span><span class="sxs-lookup"><span data-stu-id="3fa58-127">Type</span></span>        | <span data-ttu-id="3fa58-128">说明</span><span class="sxs-lookup"><span data-stu-id="3fa58-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3fa58-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3fa58-129">displayName</span></span>|<span data-ttu-id="3fa58-130">String</span><span class="sxs-lookup"><span data-stu-id="3fa58-130">String</span></span>|<span data-ttu-id="3fa58-131">publishedResource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3fa58-131">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="3fa58-132">resourceName</span><span class="sxs-lookup"><span data-stu-id="3fa58-132">resourceName</span></span>|<span data-ttu-id="3fa58-133">String</span><span class="sxs-lookup"><span data-stu-id="3fa58-133">String</span></span>|<span data-ttu-id="3fa58-134">publishedResource 的名称。</span><span class="sxs-lookup"><span data-stu-id="3fa58-134">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="3fa58-135">响应</span><span class="sxs-lookup"><span data-stu-id="3fa58-135">Response</span></span>

<span data-ttu-id="3fa58-136">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [publishedResource](../resources/publishedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3fa58-136">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3fa58-137">示例</span><span class="sxs-lookup"><span data-stu-id="3fa58-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3fa58-138">请求</span><span class="sxs-lookup"><span data-stu-id="3fa58-138">Request</span></span>

<span data-ttu-id="3fa58-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3fa58-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3fa58-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fa58-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3fa58-141">C#</span><span class="sxs-lookup"><span data-stu-id="3fa58-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-publishedresource-from-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fa58-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fa58-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-publishedresource-from-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fa58-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fa58-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-publishedresource-from-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fa58-144">Java</span><span class="sxs-lookup"><span data-stu-id="3fa58-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-publishedresource-from-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3fa58-145">响应</span><span class="sxs-lookup"><span data-stu-id="3fa58-145">Response</span></span>

<span data-ttu-id="3fa58-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3fa58-146">The following is an example of the response.</span></span>

> <span data-ttu-id="3fa58-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3fa58-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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



