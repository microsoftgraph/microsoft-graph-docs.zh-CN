---
title: '警报: updateAlerts'
description: 更新一个请求中的多个警报, 而不是多个请求。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: ad43cf3488ff0661a4b22130ae8728a00c3ea17d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322694"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="03eab-103">警报: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="03eab-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03eab-104">更新一个请求中的多个警报, 而不是多个请求。</span><span class="sxs-lookup"><span data-stu-id="03eab-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="03eab-105">权限</span><span class="sxs-lookup"><span data-stu-id="03eab-105">Permissions</span></span>

<span data-ttu-id="03eab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03eab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03eab-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="03eab-108">Permission type</span></span>                        | <span data-ttu-id="03eab-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03eab-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="03eab-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03eab-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="03eab-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03eab-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="03eab-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03eab-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="03eab-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="03eab-113">Not supported.</span></span>  |
|<span data-ttu-id="03eab-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="03eab-114">Application</span></span> | <span data-ttu-id="03eab-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03eab-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03eab-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03eab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="03eab-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="03eab-117">Request headers</span></span>

| <span data-ttu-id="03eab-118">名称</span><span class="sxs-lookup"><span data-stu-id="03eab-118">Name</span></span>          | <span data-ttu-id="03eab-119">说明</span><span class="sxs-lookup"><span data-stu-id="03eab-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03eab-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="03eab-120">Authorization</span></span> | <span data-ttu-id="03eab-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="03eab-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="03eab-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="03eab-122">Request body</span></span>

<span data-ttu-id="03eab-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="03eab-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="03eab-124">每个实体都必须具有**id**和**vendorInformation**属性。</span><span class="sxs-lookup"><span data-stu-id="03eab-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="03eab-125">有关可更新的属性的详细信息, 请参阅[更新警报](alert-update.md)。</span><span class="sxs-lookup"><span data-stu-id="03eab-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="03eab-126">参数</span><span class="sxs-lookup"><span data-stu-id="03eab-126">Parameter</span></span>    | <span data-ttu-id="03eab-127">类型</span><span class="sxs-lookup"><span data-stu-id="03eab-127">Type</span></span>        | <span data-ttu-id="03eab-128">说明</span><span class="sxs-lookup"><span data-stu-id="03eab-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03eab-129">值</span><span class="sxs-lookup"><span data-stu-id="03eab-129">value</span></span>|<span data-ttu-id="03eab-130">[通知](../resources/alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="03eab-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="03eab-131">要更新的通知的集合。</span><span class="sxs-lookup"><span data-stu-id="03eab-131">Collection of alerts to update.</span></span> <span data-ttu-id="03eab-132">每个实体都必须具有要更新的**id**、 **vendorInformation**和其他可编辑属性。</span><span class="sxs-lookup"><span data-stu-id="03eab-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="03eab-133">响应</span><span class="sxs-lookup"><span data-stu-id="03eab-133">Response</span></span>

<span data-ttu-id="03eab-134">如果成功, 此方法在`200, OK`响应正文中返回响应代码和[警报](../resources/alert.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="03eab-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03eab-135">示例</span><span class="sxs-lookup"><span data-stu-id="03eab-135">Examples</span></span>

<span data-ttu-id="03eab-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="03eab-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="03eab-137">请求</span><span class="sxs-lookup"><span data-stu-id="03eab-137">Request</span></span>

<span data-ttu-id="03eab-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03eab-138">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03eab-139">响应</span><span class="sxs-lookup"><span data-stu-id="03eab-139">Response</span></span>

<span data-ttu-id="03eab-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="03eab-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="03eab-141">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03eab-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="03eab-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="03eab-142">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
