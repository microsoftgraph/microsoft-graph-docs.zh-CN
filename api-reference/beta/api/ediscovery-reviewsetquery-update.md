---
title: 更新 reviewSetQuery
description: 更新 reviewSetQuery 对象的属性。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 863a64bd0182d43c32756b6b214753a498d400df
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515756"
---
# <a name="update-reviewsetquery"></a><span data-ttu-id="ba937-103">更新 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="ba937-103">Update reviewSetQuery</span></span>

<span data-ttu-id="ba937-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ba937-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba937-105">更新电子数据展示 [reviewSetQuery 的属性](../resources/ediscovery-reviewsetquery.md)。</span><span class="sxs-lookup"><span data-stu-id="ba937-105">Update the properties of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba937-106">权限</span><span class="sxs-lookup"><span data-stu-id="ba937-106">Permissions</span></span>

<span data-ttu-id="ba937-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba937-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba937-109">Permission type</span></span>|<span data-ttu-id="ba937-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba937-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba937-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba937-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba937-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba937-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ba937-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba937-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba937-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba937-114">Not supported.</span></span>|
|<span data-ttu-id="ba937-115">Application</span><span class="sxs-lookup"><span data-stu-id="ba937-115">Application</span></span>|<span data-ttu-id="ba937-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba937-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba937-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba937-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba937-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba937-118">Request headers</span></span>

| <span data-ttu-id="ba937-119">名称</span><span class="sxs-lookup"><span data-stu-id="ba937-119">Name</span></span>       | <span data-ttu-id="ba937-120">说明</span><span class="sxs-lookup"><span data-stu-id="ba937-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ba937-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba937-121">Authorization</span></span> | <span data-ttu-id="ba937-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba937-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba937-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba937-124">Request body</span></span>

<span data-ttu-id="ba937-125">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ba937-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ba937-126">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ba937-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ba937-127">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ba937-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ba937-128">属性</span><span class="sxs-lookup"><span data-stu-id="ba937-128">Property</span></span>     | <span data-ttu-id="ba937-129">类型</span><span class="sxs-lookup"><span data-stu-id="ba937-129">Type</span></span>        | <span data-ttu-id="ba937-130">说明</span><span class="sxs-lookup"><span data-stu-id="ba937-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ba937-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ba937-131">displayName</span></span> | <span data-ttu-id="ba937-132">String</span><span class="sxs-lookup"><span data-stu-id="ba937-132">String</span></span> | <span data-ttu-id="ba937-133">查看集查询的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ba937-133">Display name for they review set query.</span></span> |
| <span data-ttu-id="ba937-134">查询</span><span class="sxs-lookup"><span data-stu-id="ba937-134">query</span></span> | <span data-ttu-id="ba937-135">String</span><span class="sxs-lookup"><span data-stu-id="ba937-135">String</span></span> | <span data-ttu-id="ba937-136">KQL 中的查询字符串 (关键字查询语言) 查询。</span><span class="sxs-lookup"><span data-stu-id="ba937-136">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="ba937-137">有关详细信息，请参阅 ["文档元数据"字段](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。</span><span class="sxs-lookup"><span data-stu-id="ba937-137">For details, see [Document metadata fields](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span> |

## <a name="response"></a><span data-ttu-id="ba937-138">响应</span><span class="sxs-lookup"><span data-stu-id="ba937-138">Response</span></span>

<span data-ttu-id="ba937-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ba937-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba937-141">示例</span><span class="sxs-lookup"><span data-stu-id="ba937-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba937-142">请求</span><span class="sxs-lookup"><span data-stu-id="ba937-142">Request</span></span>

<span data-ttu-id="ba937-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba937-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_reviewsetquery"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
Content-type: application/json

{
  "displayName": "My Query 1 - Renamed"
}
```

### <a name="response"></a><span data-ttu-id="ba937-144">响应</span><span class="sxs-lookup"><span data-stu-id="ba937-144">Response</span></span>

<span data-ttu-id="ba937-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba937-145">The following is an example of the response.</span></span>

> <span data-ttu-id="ba937-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba937-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewsetquery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->