---
title: 创建 publishedResource
description: 创建新的**publishedResource**对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8823d80a3786ea8a8d3b1b3e1f7a1ef467e7384c
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840973"
---
# <a name="create-publishedresource"></a><span data-ttu-id="00f5c-103">创建 publishedResource</span><span class="sxs-lookup"><span data-stu-id="00f5c-103">Create publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00f5c-104">创建新的[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00f5c-104">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00f5c-105">权限</span><span class="sxs-lookup"><span data-stu-id="00f5c-105">Permissions</span></span>

<span data-ttu-id="00f5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00f5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00f5c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="00f5c-108">Permission type</span></span>                        | <span data-ttu-id="00f5c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00f5c-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="00f5c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00f5c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="00f5c-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="00f5c-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="00f5c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00f5c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00f5c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="00f5c-113">Not supported.</span></span> |
| <span data-ttu-id="00f5c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="00f5c-114">Application</span></span>                            | <span data-ttu-id="00f5c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00f5c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00f5c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00f5c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="00f5c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="00f5c-117">Request headers</span></span>

| <span data-ttu-id="00f5c-118">名称</span><span class="sxs-lookup"><span data-stu-id="00f5c-118">Name</span></span>      |<span data-ttu-id="00f5c-119">说明</span><span class="sxs-lookup"><span data-stu-id="00f5c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00f5c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00f5c-120">Authorization</span></span> | <span data-ttu-id="00f5c-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="00f5c-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="00f5c-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="00f5c-122">Request body</span></span>

<span data-ttu-id="00f5c-123">在请求正文中, 提供[publishedResource](../resources/publishedresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00f5c-123">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="00f5c-124">提供以下属性的值。</span><span class="sxs-lookup"><span data-stu-id="00f5c-124">Supply the values for the following properties.</span></span>

| <span data-ttu-id="00f5c-125">属性</span><span class="sxs-lookup"><span data-stu-id="00f5c-125">Property</span></span>     | <span data-ttu-id="00f5c-126">类型</span><span class="sxs-lookup"><span data-stu-id="00f5c-126">Type</span></span>        | <span data-ttu-id="00f5c-127">说明</span><span class="sxs-lookup"><span data-stu-id="00f5c-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="00f5c-128">displayName</span><span class="sxs-lookup"><span data-stu-id="00f5c-128">displayName</span></span>|<span data-ttu-id="00f5c-129">String</span><span class="sxs-lookup"><span data-stu-id="00f5c-129">String</span></span>|<span data-ttu-id="00f5c-130">PublishedResource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="00f5c-130">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="00f5c-131">resourceName</span><span class="sxs-lookup"><span data-stu-id="00f5c-131">resourceName</span></span>|<span data-ttu-id="00f5c-132">String</span><span class="sxs-lookup"><span data-stu-id="00f5c-132">String</span></span>|<span data-ttu-id="00f5c-133">PublishedResource 的名称。</span><span class="sxs-lookup"><span data-stu-id="00f5c-133">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="00f5c-134">响应</span><span class="sxs-lookup"><span data-stu-id="00f5c-134">Response</span></span>

<span data-ttu-id="00f5c-135">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00f5c-135">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00f5c-136">示例</span><span class="sxs-lookup"><span data-stu-id="00f5c-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00f5c-137">请求</span><span class="sxs-lookup"><span data-stu-id="00f5c-137">Request</span></span>

<span data-ttu-id="00f5c-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="00f5c-138">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00f5c-139">响应</span><span class="sxs-lookup"><span data-stu-id="00f5c-139">Response</span></span>

<span data-ttu-id="00f5c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="00f5c-140">The following is an example of the response.</span></span>

> <span data-ttu-id="00f5c-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="00f5c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
