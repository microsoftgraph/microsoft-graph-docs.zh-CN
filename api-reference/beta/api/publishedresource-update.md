---
title: 更新 publishedResource
description: 更新[publishedResource](../resources/publishedresource.md)对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e0492116ad0d012846fe1ac531ddcbf4bb77b95
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840980"
---
# <a name="update-publishedresource"></a><span data-ttu-id="4bb60-103">更新 publishedResource</span><span class="sxs-lookup"><span data-stu-id="4bb60-103">Update publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb60-104">更新 publishedresource [publishedresource](../resources/publishedresource.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4bb60-104">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bb60-105">权限</span><span class="sxs-lookup"><span data-stu-id="4bb60-105">Permissions</span></span>

<span data-ttu-id="4bb60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bb60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bb60-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bb60-108">Permission type</span></span>                        | <span data-ttu-id="4bb60-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bb60-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="4bb60-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bb60-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bb60-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="4bb60-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="4bb60-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bb60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bb60-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bb60-113">Not supported.</span></span> |
| <span data-ttu-id="4bb60-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bb60-114">Application</span></span>                            | <span data-ttu-id="4bb60-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bb60-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bb60-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bb60-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="4bb60-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bb60-117">Request headers</span></span>

| <span data-ttu-id="4bb60-118">名称</span><span class="sxs-lookup"><span data-stu-id="4bb60-118">Name</span></span>       | <span data-ttu-id="4bb60-119">说明</span><span class="sxs-lookup"><span data-stu-id="4bb60-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4bb60-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bb60-120">Authorization</span></span> | <span data-ttu-id="4bb60-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4bb60-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bb60-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bb60-122">Request body</span></span>

<span data-ttu-id="4bb60-123">在请求正文中, 提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="4bb60-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="4bb60-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="4bb60-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4bb60-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4bb60-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="4bb60-126">下表列出了可更新的属性。</span><span class="sxs-lookup"><span data-stu-id="4bb60-126">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="4bb60-127">属性</span><span class="sxs-lookup"><span data-stu-id="4bb60-127">Property</span></span>     | <span data-ttu-id="4bb60-128">类型</span><span class="sxs-lookup"><span data-stu-id="4bb60-128">Type</span></span>        | <span data-ttu-id="4bb60-129">说明</span><span class="sxs-lookup"><span data-stu-id="4bb60-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4bb60-130">displayName</span><span class="sxs-lookup"><span data-stu-id="4bb60-130">displayName</span></span>|<span data-ttu-id="4bb60-131">String</span><span class="sxs-lookup"><span data-stu-id="4bb60-131">String</span></span>|<span data-ttu-id="4bb60-132">表示内部部署的已发布资源名称。</span><span class="sxs-lookup"><span data-stu-id="4bb60-132">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="4bb60-133">响应</span><span class="sxs-lookup"><span data-stu-id="4bb60-133">Response</span></span>

<span data-ttu-id="4bb60-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4bb60-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4bb60-135">示例</span><span class="sxs-lookup"><span data-stu-id="4bb60-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4bb60-136">请求</span><span class="sxs-lookup"><span data-stu-id="4bb60-136">Request</span></span>

<span data-ttu-id="4bb60-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4bb60-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4bb60-138">响应</span><span class="sxs-lookup"><span data-stu-id="4bb60-138">Response</span></span>

<span data-ttu-id="4bb60-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4bb60-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4bb60-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4bb60-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
