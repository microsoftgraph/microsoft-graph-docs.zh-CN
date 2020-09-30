---
title: 更新 reviewSetQuery
description: 更新 reviewSetQuery 对象的属性。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: eccfd08989b9cba23d72216de441f60e10ebb00f
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314732"
---
# <a name="update-reviewsetquery"></a><span data-ttu-id="3153f-103">更新 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="3153f-103">Update reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3153f-104">更新电子数据展示 [reviewSetQuery](../resources/reviewsetquery.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="3153f-104">Update the properties of an eDiscovery [reviewSetQuery](../resources/reviewsetquery.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3153f-105">权限</span><span class="sxs-lookup"><span data-stu-id="3153f-105">Permissions</span></span>

<span data-ttu-id="3153f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3153f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3153f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3153f-108">Permission type</span></span>                        | <span data-ttu-id="3153f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3153f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3153f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3153f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3153f-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="3153f-111">User.Read</span></span> |
| <span data-ttu-id="3153f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3153f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3153f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3153f-113">Not supported.</span></span> |
| <span data-ttu-id="3153f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3153f-114">Application</span></span>                            | <span data-ttu-id="3153f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3153f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3153f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3153f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3153f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3153f-117">Request headers</span></span>

| <span data-ttu-id="3153f-118">名称</span><span class="sxs-lookup"><span data-stu-id="3153f-118">Name</span></span>       | <span data-ttu-id="3153f-119">说明</span><span class="sxs-lookup"><span data-stu-id="3153f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3153f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3153f-120">Authorization</span></span> | <span data-ttu-id="3153f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3153f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3153f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3153f-123">Request body</span></span>

<span data-ttu-id="3153f-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="3153f-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3153f-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="3153f-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3153f-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3153f-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3153f-127">属性</span><span class="sxs-lookup"><span data-stu-id="3153f-127">Property</span></span>     | <span data-ttu-id="3153f-128">类型</span><span class="sxs-lookup"><span data-stu-id="3153f-128">Type</span></span>        | <span data-ttu-id="3153f-129">说明</span><span class="sxs-lookup"><span data-stu-id="3153f-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3153f-130">displayName</span><span class="sxs-lookup"><span data-stu-id="3153f-130">displayName</span></span> | <span data-ttu-id="3153f-131">字符串</span><span class="sxs-lookup"><span data-stu-id="3153f-131">String</span></span> | <span data-ttu-id="3153f-132">他们的审阅集查询的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3153f-132">Display name for they review set query.</span></span> |
| <span data-ttu-id="3153f-133">查询</span><span class="sxs-lookup"><span data-stu-id="3153f-133">query</span></span> | <span data-ttu-id="3153f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3153f-134">String</span></span> | <span data-ttu-id="3153f-135">KQL (关键字查询语言) 查询中的查询字符串。</span><span class="sxs-lookup"><span data-stu-id="3153f-135">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="3153f-136">有关详细信息，请参阅 [Document metadata fields](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。</span><span class="sxs-lookup"><span data-stu-id="3153f-136">For details, see [Document metadata fields](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span> |

## <a name="response"></a><span data-ttu-id="3153f-137">响应</span><span class="sxs-lookup"><span data-stu-id="3153f-137">Response</span></span>

<span data-ttu-id="3153f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3153f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3153f-140">示例</span><span class="sxs-lookup"><span data-stu-id="3153f-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3153f-141">请求</span><span class="sxs-lookup"><span data-stu-id="3153f-141">Request</span></span>

<span data-ttu-id="3153f-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3153f-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_reviewsetquery"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
Content-type: application/json

{
  "displayName": "My Query 1 - Renamed"
}
```

### <a name="response"></a><span data-ttu-id="3153f-143">响应</span><span class="sxs-lookup"><span data-stu-id="3153f-143">Response</span></span>

<span data-ttu-id="3153f-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3153f-144">The following is an example of the response.</span></span>

> <span data-ttu-id="3153f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3153f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
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