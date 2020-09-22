---
title: 警报： updateAlerts
description: 更新一个请求中的多个警报，而不是多个请求。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9db39c6b7e9455e7350910eafd7ebe5ad06a5dd3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997051"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="52d1e-103">警报： updateAlerts</span><span class="sxs-lookup"><span data-stu-id="52d1e-103">alert: updateAlerts</span></span>

<span data-ttu-id="52d1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52d1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52d1e-105">更新一个请求中的多个警报，而不是多个请求。</span><span class="sxs-lookup"><span data-stu-id="52d1e-105">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="52d1e-106">权限</span><span class="sxs-lookup"><span data-stu-id="52d1e-106">Permissions</span></span>

<span data-ttu-id="52d1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52d1e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52d1e-109">Permission type</span></span>                        | <span data-ttu-id="52d1e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52d1e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="52d1e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52d1e-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="52d1e-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52d1e-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="52d1e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52d1e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="52d1e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52d1e-114">Not supported.</span></span>  |
|<span data-ttu-id="52d1e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52d1e-115">Application</span></span> | <span data-ttu-id="52d1e-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52d1e-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52d1e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52d1e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="52d1e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="52d1e-118">Request headers</span></span>

| <span data-ttu-id="52d1e-119">名称</span><span class="sxs-lookup"><span data-stu-id="52d1e-119">Name</span></span>          | <span data-ttu-id="52d1e-120">说明</span><span class="sxs-lookup"><span data-stu-id="52d1e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="52d1e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="52d1e-121">Authorization</span></span> | <span data-ttu-id="52d1e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="52d1e-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="52d1e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="52d1e-123">Request body</span></span>

<span data-ttu-id="52d1e-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="52d1e-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="52d1e-125">每个实体都必须具有 **id** 和 **vendorInformation** 属性。</span><span class="sxs-lookup"><span data-stu-id="52d1e-125">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="52d1e-126">有关可更新的属性的详细信息，请参阅 [更新警报](alert-update.md)。</span><span class="sxs-lookup"><span data-stu-id="52d1e-126">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="52d1e-127">参数</span><span class="sxs-lookup"><span data-stu-id="52d1e-127">Parameter</span></span>    | <span data-ttu-id="52d1e-128">类型</span><span class="sxs-lookup"><span data-stu-id="52d1e-128">Type</span></span>        | <span data-ttu-id="52d1e-129">说明</span><span class="sxs-lookup"><span data-stu-id="52d1e-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52d1e-130">值</span><span class="sxs-lookup"><span data-stu-id="52d1e-130">value</span></span>|<span data-ttu-id="52d1e-131">[警报](../resources/alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d1e-131">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="52d1e-132">要更新的通知的集合。</span><span class="sxs-lookup"><span data-stu-id="52d1e-132">Collection of alerts to update.</span></span> <span data-ttu-id="52d1e-133">每个实体都必须具有要更新的 **id**、 **vendorInformation**和其他可编辑属性。</span><span class="sxs-lookup"><span data-stu-id="52d1e-133">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="52d1e-134">响应</span><span class="sxs-lookup"><span data-stu-id="52d1e-134">Response</span></span>

<span data-ttu-id="52d1e-135">如果成功，此方法 `200, OK` 在响应正文中返回响应代码和 [警报](../resources/alert.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="52d1e-135">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52d1e-136">示例</span><span class="sxs-lookup"><span data-stu-id="52d1e-136">Examples</span></span>

<span data-ttu-id="52d1e-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="52d1e-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="52d1e-138">请求</span><span class="sxs-lookup"><span data-stu-id="52d1e-138">Request</span></span>

<span data-ttu-id="52d1e-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="52d1e-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52d1e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="52d1e-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="52d1e-141">C#</span><span class="sxs-lookup"><span data-stu-id="52d1e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52d1e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52d1e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52d1e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52d1e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52d1e-144">响应</span><span class="sxs-lookup"><span data-stu-id="52d1e-144">Response</span></span>

<span data-ttu-id="52d1e-145">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="52d1e-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="52d1e-146">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="52d1e-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52d1e-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="52d1e-147">All the properties will be returned from an actual call.</span></span>

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


