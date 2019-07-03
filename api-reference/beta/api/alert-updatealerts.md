---
title: '警报: updateAlerts'
description: 更新一个请求中的多个警报, 而不是多个请求。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 109767fb4d3bfaea173337a7d853e84e2261ef85
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439747"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="3e1f4-103">警报: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="3e1f4-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e1f4-104">更新一个请求中的多个警报, 而不是多个请求。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e1f4-105">权限</span><span class="sxs-lookup"><span data-stu-id="3e1f4-105">Permissions</span></span>

<span data-ttu-id="3e1f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e1f4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e1f4-108">Permission type</span></span>                        | <span data-ttu-id="3e1f4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e1f4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="3e1f4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e1f4-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="3e1f4-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e1f4-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="3e1f4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e1f4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3e1f4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-113">Not supported.</span></span>  |
|<span data-ttu-id="3e1f4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e1f4-114">Application</span></span> | <span data-ttu-id="3e1f4-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e1f4-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e1f4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e1f4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="3e1f4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e1f4-117">Request headers</span></span>

| <span data-ttu-id="3e1f4-118">名称</span><span class="sxs-lookup"><span data-stu-id="3e1f4-118">Name</span></span>          | <span data-ttu-id="3e1f4-119">说明</span><span class="sxs-lookup"><span data-stu-id="3e1f4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3e1f4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e1f4-120">Authorization</span></span> | <span data-ttu-id="3e1f4-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3e1f4-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e1f4-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e1f4-122">Request body</span></span>

<span data-ttu-id="3e1f4-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="3e1f4-124">每个实体都必须具有**id**和**vendorInformation**属性。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="3e1f4-125">有关可更新的属性的详细信息, 请参阅[更新警报](alert-update.md)。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="3e1f4-126">参数</span><span class="sxs-lookup"><span data-stu-id="3e1f4-126">Parameter</span></span>    | <span data-ttu-id="3e1f4-127">类型</span><span class="sxs-lookup"><span data-stu-id="3e1f4-127">Type</span></span>        | <span data-ttu-id="3e1f4-128">说明</span><span class="sxs-lookup"><span data-stu-id="3e1f4-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e1f4-129">值</span><span class="sxs-lookup"><span data-stu-id="3e1f4-129">value</span></span>|<span data-ttu-id="3e1f4-130">[警报](../resources/alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e1f4-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="3e1f4-131">要更新的通知的集合。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-131">Collection of alerts to update.</span></span> <span data-ttu-id="3e1f4-132">每个实体都必须具有要更新的**id**、 **vendorInformation**和其他可编辑属性。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="3e1f4-133">响应</span><span class="sxs-lookup"><span data-stu-id="3e1f4-133">Response</span></span>

<span data-ttu-id="3e1f4-134">如果成功, 此方法在`200, OK`响应正文中返回响应代码和[警报](../resources/alert.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e1f4-135">示例</span><span class="sxs-lookup"><span data-stu-id="3e1f4-135">Examples</span></span>

<span data-ttu-id="3e1f4-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3e1f4-137">请求</span><span class="sxs-lookup"><span data-stu-id="3e1f4-137">Request</span></span>

<span data-ttu-id="3e1f4-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e1f4-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3e1f4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts",
   "isCollection": "true"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": {"@odata.type": "microsoft.graph.alertFeedback"},
      "id": "String (identifier)",
      "status": {"@odata.type": "microsoft.graph.alertStatus"},
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e1f4-140">C#</span><span class="sxs-lookup"><span data-stu-id="3e1f4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e1f4-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e1f4-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e1f4-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="3e1f4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e1f4-143">响应</span><span class="sxs-lookup"><span data-stu-id="3e1f4-143">Response</span></span>

<span data-ttu-id="3e1f4-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3e1f4-145">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e1f4-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3e1f4-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
