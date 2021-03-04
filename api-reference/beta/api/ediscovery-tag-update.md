---
title: 更新标记
description: 更新标记对象的属性。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1cfc1fc24ea6e850daac08f9c741b2943b1e34d4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445983"
---
# <a name="update-tag"></a><span data-ttu-id="2e23a-103">更新标记</span><span class="sxs-lookup"><span data-stu-id="2e23a-103">Update tag</span></span>

<span data-ttu-id="2e23a-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2e23a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e23a-105">更新 [标记对象的属性](../resources/ediscovery-tag.md) 。</span><span class="sxs-lookup"><span data-stu-id="2e23a-105">Update the properties of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e23a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2e23a-106">Permissions</span></span>

<span data-ttu-id="2e23a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e23a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e23a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e23a-109">Permission type</span></span>|<span data-ttu-id="2e23a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e23a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e23a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e23a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e23a-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e23a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="2e23a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e23a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e23a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e23a-114">Not supported.</span></span>|
|<span data-ttu-id="2e23a-115">Application</span><span class="sxs-lookup"><span data-stu-id="2e23a-115">Application</span></span>|<span data-ttu-id="2e23a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e23a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e23a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e23a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="request-headers"></a><span data-ttu-id="2e23a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e23a-118">Request headers</span></span>

|<span data-ttu-id="2e23a-119">名称</span><span class="sxs-lookup"><span data-stu-id="2e23a-119">Name</span></span>|<span data-ttu-id="2e23a-120">说明</span><span class="sxs-lookup"><span data-stu-id="2e23a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2e23a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e23a-121">Authorization</span></span>|<span data-ttu-id="2e23a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e23a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2e23a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e23a-124">Content-Type</span></span>|<span data-ttu-id="2e23a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2e23a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e23a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e23a-127">Request body</span></span>

<span data-ttu-id="2e23a-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2e23a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2e23a-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2e23a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2e23a-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2e23a-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="2e23a-131">属性</span><span class="sxs-lookup"><span data-stu-id="2e23a-131">Property</span></span>|<span data-ttu-id="2e23a-132">类型</span><span class="sxs-lookup"><span data-stu-id="2e23a-132">Type</span></span>|<span data-ttu-id="2e23a-133">说明</span><span class="sxs-lookup"><span data-stu-id="2e23a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e23a-134">说明</span><span class="sxs-lookup"><span data-stu-id="2e23a-134">description</span></span>|<span data-ttu-id="2e23a-135">String</span><span class="sxs-lookup"><span data-stu-id="2e23a-135">String</span></span>|<span data-ttu-id="2e23a-136">标记的说明。</span><span class="sxs-lookup"><span data-stu-id="2e23a-136">The description for the tag.</span></span>|
|<span data-ttu-id="2e23a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2e23a-137">displayName</span></span>|<span data-ttu-id="2e23a-138">String</span><span class="sxs-lookup"><span data-stu-id="2e23a-138">String</span></span>|<span data-ttu-id="2e23a-139">标记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2e23a-139">Display name of the tag.</span></span>|

## <a name="response"></a><span data-ttu-id="2e23a-140">响应</span><span class="sxs-lookup"><span data-stu-id="2e23a-140">Response</span></span>

<span data-ttu-id="2e23a-141">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2e23a-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2e23a-142">示例</span><span class="sxs-lookup"><span data-stu-id="2e23a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e23a-143">请求</span><span class="sxs-lookup"><span data-stu-id="2e23a-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tag"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
Content-Type: application/json
Content-length: 210

{
  "description":"This is an updated description."
}
```

### <a name="response"></a><span data-ttu-id="2e23a-144">响应</span><span class="sxs-lookup"><span data-stu-id="2e23a-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
