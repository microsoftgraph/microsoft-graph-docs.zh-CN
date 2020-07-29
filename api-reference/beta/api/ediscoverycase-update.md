---
title: 更新 ediscoverycase
description: 更新 ediscoveryCase 对象的属性。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f0df9131046d8c031a492502c64c2272e4761bf0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509986"
---
# <a name="update-ediscoverycase"></a><span data-ttu-id="e1c41-103">更新 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="e1c41-103">Update ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1c41-104">更新[ediscoveryCase](../resources/ediscoverycase.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e1c41-104">Update the properties of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1c41-105">权限</span><span class="sxs-lookup"><span data-stu-id="e1c41-105">Permissions</span></span>

<span data-ttu-id="e1c41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1c41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1c41-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1c41-108">Permission type</span></span>                        | <span data-ttu-id="e1c41-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1c41-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e1c41-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1c41-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1c41-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="e1c41-111">User.Read</span></span>      |
| <span data-ttu-id="e1c41-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1c41-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1c41-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1c41-113">Not supported.</span></span> |
| <span data-ttu-id="e1c41-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1c41-114">Application</span></span>                            | <span data-ttu-id="e1c41-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1c41-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1c41-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1c41-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e1c41-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1c41-117">Request headers</span></span>

| <span data-ttu-id="e1c41-118">名称</span><span class="sxs-lookup"><span data-stu-id="e1c41-118">Name</span></span>       | <span data-ttu-id="e1c41-119">说明</span><span class="sxs-lookup"><span data-stu-id="e1c41-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e1c41-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1c41-120">Authorization</span></span> | <span data-ttu-id="e1c41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1c41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1c41-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1c41-123">Request body</span></span>

<span data-ttu-id="e1c41-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e1c41-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e1c41-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e1c41-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e1c41-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e1c41-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e1c41-127">属性</span><span class="sxs-lookup"><span data-stu-id="e1c41-127">Property</span></span>     | <span data-ttu-id="e1c41-128">类型</span><span class="sxs-lookup"><span data-stu-id="e1c41-128">Type</span></span>        | <span data-ttu-id="e1c41-129">说明</span><span class="sxs-lookup"><span data-stu-id="e1c41-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1c41-130">说明</span><span class="sxs-lookup"><span data-stu-id="e1c41-130">description</span></span>|<span data-ttu-id="e1c41-131">字符串</span><span class="sxs-lookup"><span data-stu-id="e1c41-131">String</span></span>| <span data-ttu-id="e1c41-132">事例说明。</span><span class="sxs-lookup"><span data-stu-id="e1c41-132">The case description.</span></span> |
|<span data-ttu-id="e1c41-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e1c41-133">displayName</span></span>|<span data-ttu-id="e1c41-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e1c41-134">String</span></span>| <span data-ttu-id="e1c41-135">事例名称。</span><span class="sxs-lookup"><span data-stu-id="e1c41-135">The case name.</span></span> |
|<span data-ttu-id="e1c41-136">externalId</span><span class="sxs-lookup"><span data-stu-id="e1c41-136">externalId</span></span>|<span data-ttu-id="e1c41-137">String</span><span class="sxs-lookup"><span data-stu-id="e1c41-137">String</span></span>| <span data-ttu-id="e1c41-138">Customer reference 的外部事例编号。</span><span class="sxs-lookup"><span data-stu-id="e1c41-138">The external case number for customer reference.</span></span> |

## <a name="response"></a><span data-ttu-id="e1c41-139">响应</span><span class="sxs-lookup"><span data-stu-id="e1c41-139">Response</span></span>

<span data-ttu-id="e1c41-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e1c41-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1c41-142">示例</span><span class="sxs-lookup"><span data-stu-id="e1c41-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1c41-143">请求</span><span class="sxs-lookup"><span data-stu-id="e1c41-143">Request</span></span>

<span data-ttu-id="e1c41-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1c41-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycase"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
Content-type: application/json

{
  "displayName": "My Case 1 - Renamed",
  "description": "Updated description",
  "externalId": "Updated externalId"
}
```

### <a name="response"></a><span data-ttu-id="e1c41-145">响应</span><span class="sxs-lookup"><span data-stu-id="e1c41-145">Response</span></span>

<span data-ttu-id="e1c41-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1c41-146">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ediscoverycase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
