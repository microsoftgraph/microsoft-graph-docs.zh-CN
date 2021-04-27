---
title: 警报：updateAlerts
description: 更新一个请求而不是多个请求中的多个警报。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 86c391f0684ebad30ef5abab0c3a7e8746445a32
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048181"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="247d5-103">警报：updateAlerts</span><span class="sxs-lookup"><span data-stu-id="247d5-103">alert: updateAlerts</span></span>

<span data-ttu-id="247d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="247d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="247d5-105">更新一个请求而不是多个请求中的多个警报。</span><span class="sxs-lookup"><span data-stu-id="247d5-105">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="247d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="247d5-106">Permissions</span></span>

<span data-ttu-id="247d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="247d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="247d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="247d5-109">Permission type</span></span>                        | <span data-ttu-id="247d5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="247d5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="247d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="247d5-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="247d5-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="247d5-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="247d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="247d5-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="247d5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="247d5-114">Not supported.</span></span>  |
|<span data-ttu-id="247d5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="247d5-115">Application</span></span> | <span data-ttu-id="247d5-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="247d5-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="247d5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="247d5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="247d5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="247d5-118">Request headers</span></span>

| <span data-ttu-id="247d5-119">名称</span><span class="sxs-lookup"><span data-stu-id="247d5-119">Name</span></span>          | <span data-ttu-id="247d5-120">说明</span><span class="sxs-lookup"><span data-stu-id="247d5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="247d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="247d5-121">Authorization</span></span> | <span data-ttu-id="247d5-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="247d5-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="247d5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="247d5-123">Request body</span></span>

<span data-ttu-id="247d5-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="247d5-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="247d5-125">每个实体必须具有 **id** 和 **vendorInformation** 属性。</span><span class="sxs-lookup"><span data-stu-id="247d5-125">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="247d5-126">有关可更新的属性的详细信息，请参阅 [更新警报](alert-update.md)。</span><span class="sxs-lookup"><span data-stu-id="247d5-126">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="247d5-127">参数</span><span class="sxs-lookup"><span data-stu-id="247d5-127">Parameter</span></span>    | <span data-ttu-id="247d5-128">类型</span><span class="sxs-lookup"><span data-stu-id="247d5-128">Type</span></span>        | <span data-ttu-id="247d5-129">说明</span><span class="sxs-lookup"><span data-stu-id="247d5-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="247d5-130">值</span><span class="sxs-lookup"><span data-stu-id="247d5-130">value</span></span>|<span data-ttu-id="247d5-131">[警报](../resources/alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="247d5-131">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="247d5-132">要更新的警报集合。</span><span class="sxs-lookup"><span data-stu-id="247d5-132">Collection of alerts to update.</span></span> <span data-ttu-id="247d5-133">每个实体必须具有 **id** **、vendorInformation** 和其他可编辑属性以进行更新。</span><span class="sxs-lookup"><span data-stu-id="247d5-133">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="247d5-134">响应</span><span class="sxs-lookup"><span data-stu-id="247d5-134">Response</span></span>

<span data-ttu-id="247d5-135">如果成功，此方法在 `200, OK` 响应正文中返回 [响应](../resources/alert.md) 代码和 alert 集合对象。</span><span class="sxs-lookup"><span data-stu-id="247d5-135">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="247d5-136">示例</span><span class="sxs-lookup"><span data-stu-id="247d5-136">Examples</span></span>

<span data-ttu-id="247d5-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="247d5-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="247d5-138">请求</span><span class="sxs-lookup"><span data-stu-id="247d5-138">Request</span></span>

<span data-ttu-id="247d5-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="247d5-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="247d5-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="247d5-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="247d5-141">C#</span><span class="sxs-lookup"><span data-stu-id="247d5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="247d5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="247d5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="247d5-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="247d5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="247d5-144">Java</span><span class="sxs-lookup"><span data-stu-id="247d5-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/alert-updatealerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="247d5-145">响应</span><span class="sxs-lookup"><span data-stu-id="247d5-145">Response</span></span>

<span data-ttu-id="247d5-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="247d5-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="247d5-147">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="247d5-147">The response object shown here might be shortened for readability.</span></span>

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


